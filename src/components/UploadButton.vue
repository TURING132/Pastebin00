<script>
import { defineComponent } from "vue";
import { useMessage,NButton,NUpload } from "naive-ui";

export default defineComponent({
    components:{
        NButton,
        NUpload
    },
  setup() {
    let support=[   'pdf',
                    'txt',
                    'c','cpp','cxx','txx','c++','C','cc','h','hpp','hxx',
                    'cs',
                    'java','class',
                    'py','py3',
                    'js',
                    'go',
                    ]
    const message = useMessage();
    return {
      async beforeUpload(data) {
          console.log(data);
        let filename = data.file.file.name.split('.').pop().toLowerCase();
        let correctFile = false;
        support.forEach(element => {
            if(element==filename){
                correctFile=true
            }
        });
        if (!correctFile) {
          message.error("只能上传pdf,txt,C,C++,C#,Java,Python,JS,Goland文件，请重新上传");
          return false;
        }
        return true;
      }
    };
  }
});
</script>

<template>
  <n-upload
    multiple
    :max="1"
    action="https://www.mocky.io/v2/5e4bafc63100007100d8b70f"
    @before-upload="beforeUpload"
  >
    <n-button strong secondary type="tertiary">upload file</n-button>
  </n-upload>
</template>