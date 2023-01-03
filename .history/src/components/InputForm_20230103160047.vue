<template>
<p>Name: </p>
<input type="text" placeholder="Name" v-model="">
</template>

<script>
export default {
data(){
    return {
        myObject:{
            fullName:"",
        
    }
}
}
</script>