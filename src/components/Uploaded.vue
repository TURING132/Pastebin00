<script setup>
    
</script>
<template>
    <div class="Uploaded-wrapper">
        <div class="Uploaded-center-wrapper">
            <slot>
                <!-- 插槽，留给设置选项 -->
            </slot>
            uploaded(hide initially)
        </div>
    </div>
</template>
<style scoped>
    .Uploaded-wrapper{
        /* background-color: blue; */
        position: relative;
        height: 315px;
    }
    .Uploaded-wrapper .Uploaded-center-wrapper{
        /* background-color: hotpink; */
        width: 70%;
        height: 300px;
        position: absolute;
        left: 50%;
        margin:  15px -35%;
        border: 1px rgb(221, 221, 221) solid;
    }

</style>

