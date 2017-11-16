<template>
	<div class="inputform">
		<span>title:</span>
		<input type="text" v-model="newtitle" >
		<span>content:</span>
		<input type="text" v-model="newcontent">
		<button v-on:click="addtodo"> Add Item </button>
	</div>
</template>
<script>
export default {

	data () {
		return {
			newtitle:"",
			newcontent:"",			
		}
	},
	methods: {
		addtodo() {

		}
	}
}
</script>