<template>
	<div class="postlist">
		<PostItem v-for="todo in todos" :todo.sync="todo" />
	</div>
</template>
<script>
import PostItem from "@/components/PostItem";
export default {
	props: ['todos'],
	data () {

	},
	components: {
		PostItem
	}
}

</script>