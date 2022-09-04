<template>
  <div>
<!--    头部-->
    <Header />

<!--    主体-->
    <div style="display: flex">
<!--      侧边栏-->
      <Aside />
<!--      内容-->
        <router-view style="flex: 1"/>

    </div>
  </div>
  <router-view/>
</template>

<style>

</style>

<script>
  import Header from "@/components/Header";
  import Aside from "@/components/Aside";

  export default {
    name: "Layout",
    components: {
      Header,//引入Header
      Aside//引入Aside
    }
  }
</script>