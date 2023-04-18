<template>
    <div>
        <button @click="text1='Javascript'">Javascript</button>
        <button @click="text1='NodeJs'">node</button>
        
    </div>
<br/>
    <component :is='text1'/>
</template>
<script>
import Javascript from './Javascript.vue'
import NodeJs from './NodeJs.vue'
export default {
  components: { NodeJs, Javascript },
    name:'DynamicComponen',
    data() {
        return {
            text1:'Javascript'
        }
    },
}
</script>