<template>
    <div>
        <input type="text" v-model="data">
        {{data}}
    </div>
</template>
<script>
export default {
    data(){
        return{
            data:2
        }
    }
}
</script>