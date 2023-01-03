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

<div v-for="item in checkBoxList" :key="item.id">
<input type="checkbox" v-model="myObject.c">
<label for="checkbox">{{ item.title }}</label>
</div>

<div v-for="item in checkBoxList" :key="item" >
<input type="radio" v-model="myObject" :value="item.value" id="item.value">
<label >{{ item.title }}</label>
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
            checkBox:[],
        },
        checkBoxList:[
            {id: 1, title:"Apple", isCheckKed:false, value: "apple"},
            {id: 2,title:"Orange", isCheckKed:false, value: "orange"},
            {id: 3,title:"Mango", isCheckKed:false, value: "mango"},
            {id: 4,title:"Kiwi", isCheckKed:false, value: "kiwi"},
            {id: 5,title:"Water Lemon", isCheckKed:false, value: "water lemon"},
            {id: 6,title:"Lemon", isCheckKed:false, value: "lemon"},
            ],
        }
    }
}
</script>