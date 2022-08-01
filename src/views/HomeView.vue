<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
  <Navigasi/>
  <Banner/>
  <Tentang/>
  <Pelayanan/>
  <Portofolio/>
  <TimKami/>
  <!-- <Blog/> -->
  <KontakKami/>
  <MyFooter/>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Navigasi from '@/components/Navigasi.vue'
import Banner from '@/components/Banner.vue'
import Tentang from '@/components/Tentang.vue'
import Pelayanan from '@/components/Pelayanan.vue'
import Portofolio from '@/components/Portofolio.vue'
import TimKami from '@/components/TimKami.vue'
// import Blog from '@/components/Blog.vue'
import KontakKami from '@/components/KontakKami.vue'
import MyFooter from '@/components/MyFooter.vue'

export default {
  name: 'HomeView',
  components: {
    // HelloWorld,
    Navigasi,
    Banner,
    Tentang,
    Pelayanan,
    Portofolio,
    TimKami,
    // Blog,
    KontakKami,
    MyFooter,
  }
}
</script>
