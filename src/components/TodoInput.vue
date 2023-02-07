<template>
  <div>
    <input type="text" v-model="newTodoItem">
    <button v-on:click="addTodo">+</button>
  </div>
</template>

<script>
export default {
  data: function(){
    return {
      newTodoItem: "",
    }
  },
  methods: {
    addTodo: function(){
      console.log(this.newTodoItem);
      //저장하는 로직
      this.newTodoItem = '';
    }
  }
}
</script>

<style>

</style>