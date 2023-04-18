<template v-if="true">
 <div>
   <ParentChild />
   <br/>
  <DynamicComponen/>
 </div>
</template>

<script>
import DynamicComponen from './assets/components/DynamicComponen.vue';
import ParentChild from "./assets/components/ParentChild.vue";
export default {
  components: { ParentChild, DynamicComponen },
  name: "App",
};
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
</style>
