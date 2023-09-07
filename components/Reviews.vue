<template>
	<section class="reviews">

		<h2 class="typo-t2 reviews__title js-reviews__title">Reviews</h2>

		<div class="container">
			<div class="reviews__list">
				<review-card
					v-for="review in reviews"
					:key="review.author"
					:author="review.author"
					:company="review.company"
					:review="review.review"
					:link="review.link"
					:imgSrc="review.imgSrc"
					:imgAlt="`${review.author} review`"
				>
				</review-card>
			</div>
			<div class="clear"></div>
		</div>
		<!-- // -->
	</section>
</template>

<script>
import reviews from '../data/reviews.json'
import ReviewCard from '~/components/ReviewCard.vue'

export default {
	name: 'NuxtReviews',
	components: {
		ReviewCard,
  	},
	data() {
		return {
			reviews,
		}
	},
}
</script>
<style lang="scss">
.reviews {
	position: relative;

	&__title {
		top: 50%;
		position: sticky;
		text-align: center;
		z-index: 2;
	}

	&__list {
		max-width: 770px;
		margin: auto;
	}
}
</style>