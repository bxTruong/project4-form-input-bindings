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
<div v-for="item in checkBoxList" v-ke>
<input type="checkbox" v-model="myObject.checked">
<label for="checkbox">{{ myObject.checked }}</label>
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
            checkBoxModel(title="Apple", isCheckKed=false),
            checkBoxModel(title="Lemon", isCheckKed=false),
            checkBoxModel(title="Water Lemon", isCheckKed=false),
            checkBoxModel(title="Mango", isCheckKed=false),
        ]
    }
}
}
</script>