<template>
  <div>
    <p>Loop the data</p>
  
<!-- example-1 -->
    <div v-for="item in arr" :key="item">
      {{ item }}
    </div>
<!-- example-1 -->  <br />
 <div v-for="item of arr2" :key="item.id">
      {{ item.name }}
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      arr: ["Vue", "Node", "Mongo"],
      arr2: [{id:1,name:'Javascript'}, {id:2,name:'HTML'},{id:2,name:'Css'}],
    };
  },
};
</script>