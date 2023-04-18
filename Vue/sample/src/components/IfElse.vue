<template>
    <div>
        <button @click="showData">{{hideData?  'Hide Data' : 'Show Data'}}</button>
    </div>
</template>
<script>
export default {
    name:'IfElse',
    props:{
        showData:Function,
        hideData:String
    }
}
</script>