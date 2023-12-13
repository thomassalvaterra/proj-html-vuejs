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
	data() {
		return {
			footerLinks: [
				{
					title: [
						{
							type: "Movie Category"
						},
					],
					link: [
						{
							type: "English New Movie"
						},
						{
							type: "Hindi All Movie"
						},
						{
							type: "Latest Tamil Movie"
						},
						{
							type: "New Top Rating Movie"
						},
						{
							type: "Hornn New Movie"
						},
						{
							type: "Animation New Movie"
						}
					]

				},
				{
					title: [
						{
							type: "Information",
						}
					],
					link: [
						{
							type: "Youtube Video Post"
						},
						{
							type: "Actor Information"
						},
						{
							type: "New Promotion"
						},
						{
							type: "Latest Movie In English"
						},
						{
							type: "Latest Flim Product"
						},
						{
							type: "Video New Video"
						}
					]

				},
			]
		}
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
	<div class="container">
		<PageOtherCards />
	</div>
	<div class="container">
		<PageLatestMovie />
	</div>
	<div class="container">
		<PageInput />
	</div>
	<div class="bg-img2">
		<div class="container">
			<div class="row">
				<div class="col-3">
					<h6><b>About Us</b></h6>
					<p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Exercitationem laboriosam error magni amet,
						sed
						doloremque fugit vero repellendus nulla corporis ipsum neque. Dolorem corporis necessitatibus cum
						pariatur
						sapiente est dolore?
					</p>
					<span class="ml"><a href="#"><i class="fa-brands fa-facebook m-star lock fb"></i></a><a href="#"><i
								class="fa-brands fa-twitter m-star lock tw"></i></a><a href="#"><i
								class="fa-brands fa-linkedin m-star lock lk"></i></a><a href="#"><i
								class="fa-brands fa-instagram m-star lock ig"></i></a><a href="#"><i
								class="fa-brands fa-google-plus-g m-star lock gp"></i></a></span>
				</div>
				<div class="col-3">
					<PageFooter v-for="link in footerLinks" :links="link" />
				</div>
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

.bg-img2 {
	background-image: url(./assets/ft-bg.jpg);
	width: 100%;
	height: 450px;
	object-fit: cover;
}
</style>
