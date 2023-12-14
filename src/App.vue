<script>
import PageHeader from './components/PageHeader.vue';
import PageJumbo from './components/PageJumbo.vue';
import PageNewMovie from './components/PageNewMovie.vue';
import PageMoviePlaylist from './components/PageMoviePlaylist.vue';
import PageCountdown from './components/PageCountdown.vue';
import PageOtherCards from './components/PageOtherCards.vue';
import PageLatestMovie from './components/PageLatestMovie.vue';
import PageInput from './components/PageInput.vue';
import PageFooter from './components/PageFooter.vue';

export default {
	components: {
		PageHeader,
		PageJumbo,
		PageNewMovie,
		PageMoviePlaylist,
		PageCountdown,
		PageOtherCards,
		PageLatestMovie,
		PageInput,
		PageFooter
	},
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
	<div class="container">
		<PageOtherCards />
	</div>
	<div class="container">
		<PageLatestMovie />
	</div>
	<div class="container">
		<PageInput />
	</div>
	<div class="d-flex">
		<PageFooter />
	</div>
	<div class="container">
		<div class="d-flex justify-content-between">
			<div>
				<span class="fs-12 mr-10"><a href="#">Term And Conditions</a></span>
				<span class="fs-12 mr-10"><a href="#">Policy</a></span>
				<span class="fs-12 mr-10"><a href="#">About</a></span>
			</div>
			<div>
				<span class="fs-12">2020 <span><a href="#">@Themepul</a></span> All Rights Reserved.</span>
			</div>
		</div>

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

.fs-12 {
	font-size: 12px;
}

a {
	color: white;
	text-decoration: none;
}

a:hover {
	color: rgb(19, 190, 19);
}

.mr-10 {
	margin-right: 10px;
}
</style>
