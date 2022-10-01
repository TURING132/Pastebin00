<script setup>
  import { NDivider } from 'naive-ui'
</script>

<template>
    <header>
        <div class="title-wrapper">
            <h1 class="title">PasteBin</h1>
            <n-divider />
        </div>
        <p class="discription">
        This is a PasteBin.
        <br>
        <span class="bold">Usage</span> : Code text or upload a file, click submit button, and get an <span class="gray">URL</span>.
        <br>
        With the <span class="gray">URL</span> you can share it.
    </p>
    </header>
</template>

<style scoped>
    *{
        box-sizing: border-box;
    }
    header{
        position: relative;
        height: 220px;
        width: 100%;
        /* background-color: aqua; */
    }
    .title-wrapper{
        /* background-color: blue; */
        height: 100px;
        width: 70%;
        position: absolute;
        left: 50%; top: 50%;
        margin: -75px 0 0 -35%;
    }
    .title-wrapper .title{
        font-size: 50px;
    }
    .discription{
        /* background-color: blueviolet; */
        height: 90px;
        width: 70%;
        position: absolute;
        left: 50%; top: 50%;
        margin: 0 0 0 -35%;
        line-height: 30px;
        font-size: 18px;
    }
    .discription .bold{
        font-weight: 900;
    }
    .discription .gray{
        color: gray;
    }

</style>