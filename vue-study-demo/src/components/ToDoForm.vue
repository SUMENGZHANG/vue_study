<template>
  
  <form  @submit.prevent="onSubmit">
    <label for="new-todo-input"> What needs to be done? </label>
    <input
      type = "text"
      id = "new-todo-input"
      name = "new-todo"
      autocomplete="off"
      v-model="label"
    />
    <button type = "submit">Add</button>
    </form>
</template>

<script>
  export default {
    
    data(){
         return {
            label:"",
         }
    },

    methods:{
        onsubmit(){
            console.log("label value",this.label)
        }
    }
  };
</script>