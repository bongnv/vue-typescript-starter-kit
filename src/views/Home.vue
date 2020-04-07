<template>
  <div class="home">
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script lang="ts">
// @ is an alias to /src
import Vue from "vue";
import HelloWorld from "@/components/HelloWorld.vue";
import appConfig from "@/app.config.json";

export default Vue.extend({
  name: "Home",
  metaInfo: {
    title: "Home",
    meta: [{ name: "description", content: appConfig.description }]
  },
  components: {
    HelloWorld
  }
});
</script>
