<template>
  <div class="todos">
    <h1>Todo App</h1>

    <input @keyup.enter="add" type="text" v-model="title" placeholder="What you want to do" />
    <button @click="add">Add to list</button>
	<ul>
		<li v-for="todo in todos" v-bind:key="todo">{{todo}}</li>
	</ul>
  </div>
</template>

<script>
export default {
  name: 'todo',
  props: {
    msg: String,
  },
	data(){
		return{
			title: '',
			todos:[
				"Go to shop"
			]
		}
	},
	methods: {
		add(){
			this.todos.push(this.title);
			this.title = "";
		}
	}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss"></style>
