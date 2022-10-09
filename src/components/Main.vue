<script setup>
    import {NButton} from 'naive-ui'
    import {NUpload} from 'naive-ui'
</script>
<template>
    <div class="main-wrapper">
        <div class="button-bar">
            <n-button strong secondary type="tertiary">
                &nbsp;Edit text&nbsp;
            </n-button>
            <n-upload
                action="请求提交的地址"
                    :headers="{//HTTP 请求需要附加的 Headers
                    'naive-info': 'hello!'//提交表单需要附加的数据
                    }"
                    :data="{
                    'naive-data': 'cool! naive!'
                    }"
                >
                <n-button strong secondary type="tertiary">
                    Upload File
                </n-button>
            </n-upload>
        </div>
        <div class="text-area">
            <textarea id="paste-panel" placeholder="Put your paste here" name="input" cols="100" rows="10"></textarea>     
        </div>
    </div>
</template>
<style scoped>
    .main-wrapper{
        /* background-color: green; */
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;

        width: 70%;
        margin:10px;
        box-sizing: border-box;
        border:1px solid black;
    }
    .button-bar{
        display: flex;
        flex-direction: row;
        
        width: 100%;
        
        border:1px solid black;
    }
    .text-area{
        width: 100%;
        display: flex;

        padding:1px;
        border: 1px rgb(221, 221, 221) solid;
    }
    textarea{
        resize: vertical;

        width: 100%;

        border:transparent;
        outline:none;
    }
</style>