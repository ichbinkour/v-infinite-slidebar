<template>
  <div>
    <v-infinite-slidebar
      :slideBarStyle="{
        background: '#42b883',
        padding: '5px 0',
      }"
      duration="10s"
    >
      <span>coucou</span>
      <span>coucou</span>
      <span>coucou</span>
      <span>coucou</span>
      <span>coucou</span>
    </v-infinite-slidebar>
  </div>
</template>

<script>
import VInfiniteSlidebar from "../src/v-infinite-slidebar";

export default {
  name: "app",
  components: {
    VInfiniteSlidebar,
  },
};
</script>

<style>
body {
  margin: 0px;
}
</style>
