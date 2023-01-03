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

<div v-for="item in checkBoxList" :key="item.title">
<input type="checkbox" v-model="item.isCheckKed">
<label for="checkbox">{{ item.title }}</label>
</div>

<div v-for="item in checkBoxList" :key="item.title" >
<input type="checkbox" v-model="item.isCheckKed" value="">
<label for="checkbox">{{ item.title }}</label>
</div>

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
        },
        checkBoxList:[
            {title:"Apple", isCheckKed:false, value: "apple"},
            {title:"Orange", isCheckKed:false, value: "orange"},
            {title:"Mango", isCheckKed:false, value: "mango"},
            {title:"Kiwi", isCheckKed:false, value: "apple"},
            {title:"Water Lemon", isCheckKed:false, value: "apple"},
            {title:"Lemon", isCheckKed:false, value: "apple"},
            ],
        }
    }
}
</script>