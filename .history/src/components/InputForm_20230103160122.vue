<template>
<p>Name: </p>
<input type="text" placeholder="Name" v-model="myObject.fullName">
<p>Name: </p>
<input type="text" placeholder="Name" v-model="myObject.fullName"><p>Name: </p>
<input type="text" placeholder="Name" v-model="myObject.fullName">
</template>

<script>
export default {
data(){
    return {
        myObject:{
            fullName:"",
            birthDay:"",
            email:"",
        }
    }
}
}
</script>