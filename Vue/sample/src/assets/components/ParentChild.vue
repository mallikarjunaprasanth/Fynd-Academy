<template>
  <div>
      <div>
    
      <!-- if else condition -->
      <IfElse :showData="hideBtn" :hideData="hideData" />
    </div>
      <br />
    <div v-if="hideData">



      <ChildParent :inc="count" :dec="childToParent" />


      
      <br />
      <button @click="parent()">This is parent to child count</button>
      <br />
      <div>
        <br />
        <!-- two way data binding -->
        <p>two way data binding</p>
        <TwoWayBinding />
      </div>
      <br />
      <br />
      <!-- for loop -->
      <div>
        <ForLoop />
      </div>
    </div>
    <div v-else>No Data to show</div>
  </div>
</template>
<script>
import ChildParent from "./ChildParent.vue";
import ForLoop from "./ForLoop.vue";
import IfElse from "./IfElse.vue";
import TwoWayBinding from "./TwoWayBinding.vue";

export default {
  name: "ParentChild",
  components: { ChildParent, TwoWayBinding, IfElse, ForLoop },
  data() {
    return {
      count: 0,
      hideData: false,
    };
  },
  methods: {
    parent() {
      this.count += 1;
    },
    childToParent() {
      this.count -= 1;
    },
    hideBtn() {
      this.hideData = !this.hideData;
    },
  },
};
</script>
<style >
</style>