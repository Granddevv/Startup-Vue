<template>
	<div class="item">
		<div class="hideform" v-show="isenable">
			<h6>{{todo.title}}</h6>
			<h6>{{todo.content}}</h6>
			<button v-on:click="showform">show</button>
			<button v-on:click="completeitem">Complete </button>
			<button v-on:click="deleteitem"> X </button>

		</div>
		<div class="showform" v-show="!isenable">
			<input v-model="todo.title">
			<input v-model="todo.content">
			<button v-on:click="hideform">hide</button>
		</div>
	</div>
</template>
<script>
	export default {
		props: ['todo'],
		data () {
			return {
				isenable:false,
			}
		},
		methods: {
			showform() {
				this.isenable=false;
			},
			hideform() {
				this.isenable=true;
			}
		}

	}
</script>
<style scoped>
	.hideform {
		display:inline-flex;
	}
	.showform {

	}
</style>
