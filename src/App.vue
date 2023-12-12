<script>
import PageHeader from './components/PageHeader.vue';
import PageJumbo from './components/PageJumbo.vue';
import PageNewMovie from './components/PageNewMovie.vue';
import PageMoviePlaylist from './components/PageMoviePlaylist.vue';
import PageCountdown from './components/PageCountdown.vue';
import PageFooter from './components/PageFooter.vue';

export default {
	components: {
		PageHeader,
		PageJumbo,
		PageNewMovie,
		PageMoviePlaylist,
		PageCountdown,
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
		<PageNewMovie />
	</div>
	<div class="container">
		<PageMoviePlaylist />
	</div>
	<PageCountdown />
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
