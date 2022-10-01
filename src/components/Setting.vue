<script setup>
    
</script>
<template>
    <div class="Setting-wrapper">
        <div class="Setting-center-wrapper">
            <slot>
                <!-- 插槽，留给设置选项 -->
            </slot>
            setting
        </div>
    </div>
</template>
<style scoped>
    .Setting-wrapper{
        /* background-color: blue; */
        position: relative;
        height: 365px;
    }
    .Setting-wrapper .Setting-center-wrapper{
        /* background-color: hotpink; */
        width: 70%;
        height: 350px;
        position: absolute;
        left: 50%;
        margin:  15px -35%;
        border: 1px rgb(221, 221, 221) solid;
    }

</style>

