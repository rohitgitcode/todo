
<template>

<p>Hello To do</p>
<input v-model="task" placeholder="enter something">
<button @click="addtask">Add Task</button>
<div >{{arr}}</div>



</template>

<script setup>
import { ref } from 'vue'

let task = ref('')
let arr = ref([])

function addtask(){
   arr.value.push(task.value)
   task.value = ''
}




</script>