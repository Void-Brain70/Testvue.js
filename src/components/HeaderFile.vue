<template>
   <div>
    <p Firstname: {{firstName}} ></p>
    <p Lastname: {{lastName}} ></p>
    <p ID: {{id}} ></p>
    <button @click= "updateName" >Click</button>
   </div>
</template>


<script>
export default{
    name: "HaderFile",
    propos:{
        firstName: String,
        lastName: String,
        id: Number
    },
    methods:{
        updateName(){
            this.$emit('updateValue','Anik');
        }
    }
}
</script>

<style scoped>
    div{
        color: violet;
    }
</style>