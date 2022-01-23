<template>
  <div id="wrapper">
    <Header />
      <div class="main">
          <MenuSidebar/>
          <Content/>
      </div>

    <Copyright />
  </div>
</template>

<script>
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'
import Header from '@/components/Header.vue'
import MenuSidebar from '@/components/MenuSidebar.vue'
import Content from '@/components/Content.vue'
import Copyright from '@/components/Copyright.vue'

export default {
  name: 'App',
  components: {
      Header,
      MenuSidebar,
      Content,
      Copyright,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

Header {
    z-index: 10;
    position: relative;
}

.main {
    display: flex;
    z-index: 10;
    background: #f1f4f6;
}

Content {
    background: #f1f4f6;
    background-size: cover;
    max-width: 1200px;
}

#wrapper > div.main > div:nth-child(2){
    margin: 0 auto;

}

MenuSidebar {
    position: absolute;
}
.sidebar {
    width: 65px;

}

.content {

}

</style>
