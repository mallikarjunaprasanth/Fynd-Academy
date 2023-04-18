<template>
    <div>
        <h1>{{inc}}</h1>
        <button @click='dec'>dec-child-to-parent</button>
    </div>
</template>
<script>
export default {
    name:'ChildParent',
     props:{
        inc:Number,
        dec:Function
  }
}
</script>