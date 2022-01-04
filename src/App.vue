<template>
  <div >
    <Header></Header>
    <div disabled="flex">
      <Aside></Aside>
      <Main></Main>
    </div>
  </div>
  <router-view/>
</template>

<style>

</style>
<script>
import Header from "@/components/Header";
import Aside from "@/components/Aside";
import Main from "@/components/Main";
export default {
  components: {Main, Aside, Header}
}
</script>