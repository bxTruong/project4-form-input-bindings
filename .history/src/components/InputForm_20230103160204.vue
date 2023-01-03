<template>
<p>Name: </p>
<input type="text" placeholder="Name" v-model="myObject.fullName">
<p>Name: </p>
<input type="text" placeholder="Birth day" v-model="myObject.birthDay">
<p>Name: </p>
<input type="text" placeholder="Email" v-model="myObject.fullName">
</template>

<script>
export default {
data(){
    return {
        myObject:{
            fullName:"",
            birthDay:"",
            email:"",
            phone:"",
        }
    }
}
}
</script>