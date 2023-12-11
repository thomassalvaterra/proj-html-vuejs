<script>
import PageHeader from './components/PageHeader.vue';
import PageMain from './components/PageMain.vue';
import PageFooter from './components/PageFooter.vue';

export default {
	components: {
		PageHeader,
		PageMain,
		PageFooter
	}
}
</script>

<template>
	<div class="container">
		<PageHeader />
	</div>
</template>

<style scoped>
.container {
	width: 1000px;
	margin: 0 auto;
}
</style>
