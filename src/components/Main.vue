<script setup>
    import {NButton,NMessageProvider} from 'naive-ui'
    import UploadButton from './UploadButton.vue'
</script>
<template>
    <div class="main-wrapper">
        <div class="button-bar">
            <n-button strong secondary type="tertiary">
                &nbsp;Edit text&nbsp;
            </n-button>
            <n-message-provider>
            <UploadButton/>
            </n-message-provider>
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
        height:36px;
        
        border:1px solid black;
    }
    .text-area{
        width: 100%;
        display: flex;

        padding:1px;
        box-sizing: border-box;
        border: 1px rgb(221, 221, 221) solid;
    }
    textarea{
        resize: vertical;

        width: 100%;

        border:transparent;
        outline:none;
    }
</style>