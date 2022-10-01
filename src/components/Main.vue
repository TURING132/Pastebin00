<script setup>
    import {NButton} from 'naive-ui'
</script>
<template>
    <div class="main-wrapper">
        <div class="text-wrapper">
            <div class="button-bar">
                <n-button strong secondary type="tertiary">
                    &nbsp;Edit text&nbsp;
                </n-button>
                <n-button strong secondary type="tertiary">
                    Upload File
                </n-button>
            </div>
            <div class="text-area">
                <slot name='text'>
                    <!-- 插槽，留给代码输入&高亮 -->
                </slot>
            </div>
        </div>
    </div>
</template>
<style scoped>
    .main-wrapper{
        /* background-color: green; */
        position: relative;
        height: 600px;
    }
    .main-wrapper .text-wrapper{
        /* background-color: hotpink; */
        width: 70%;
        height: 600px;
        position: absolute;
        left: 50%;
        margin:  0 -35%;
    }
    .text-wrapper .text-area{
        height: 565px;
        border: 1px rgb(221, 221, 221) solid;
    }
</style>