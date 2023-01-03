<template>
<p>Name: {{ myObject.fullName }}</p>
<input type="text" placeholder="Name" v-model="myObject.fullName">
<p>Birth day: {{ myObject.birthDay }}</p>
<input type="text" placeholder="Birth day" v-model="myObject.birthDay">
<p>Email: {{ myObject.email }}</p>
<input type="email" placeholder="Email" v-model="myObject.email">
<p>Phone: {{ myObject.phone }}</p>
<input type="number" placeholder="Phone" v-model="myObject.phone">
<br/>
<input type="checkbox" v-model="myObject.checked">
<label for="checkbox">{{ checked }}</label>

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
            checked:false,
        }
    }
}
}
</script>