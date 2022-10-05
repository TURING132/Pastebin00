<script setup>
  import Header from './components/Header.vue'
  import Main from './components/Main.vue'
  import Setting from './components/Setting.vue'
  import Uploaded from './components/Uploaded.vue'
  import Submit from "./components/Submit.vue"
</script>
<template>
  <div class="App">
    <Header></Header>
    <Main></Main>
    <Setting></Setting>
    <Uploaded></Uploaded>
    <Submit></Submit>
    <footer></footer>
  </div>
</template>InputSetting

<style scoped>
  footer{
    position: relative;
    height: 80px;
  }
  .App{
    display: flex;
    flex-direction: column;
    align-items: center;
  }
</style>