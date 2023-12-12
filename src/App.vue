<script>
import PageHeader from './components/PageHeader.vue';
import PageJumbo from './components/PageJumbo.vue';
import PageMovie from './components/PageMovie.vue';
import PageFooter from './components/PageFooter.vue';

export default {
	components: {
		PageHeader,
		PageJumbo,
		PageMovie,
		PageFooter
	}
}
</script>

<template>
	<div class="container">
		<PageHeader />
	</div>
	<PageJumbo />
	<div class="container">
		<PageMovie />
	</div>
</template>

<style lang="scss">
@use './styles/general.scss';
</style>

<style scoped>
.container {
	width: 1000px;
	margin: 0 auto;
}
</style>
