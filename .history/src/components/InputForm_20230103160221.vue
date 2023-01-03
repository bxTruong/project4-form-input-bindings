<template>
<p>Name: </p>
<input type="text" placeholder="Name" v-model="myObject.fullName">
<p>Name: </p>
<input type="text" placeholder="Birth day" v-model="myObject.birthDay">
<p>Email: </p>
<input type="email" placeholder="Email" v-model="myObject.email">
<p>Phone: </p>
<input type="email" placeholder="Email" v-model="myObject.email">
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