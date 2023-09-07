<template>
	<section class="reviews">

		<h2 class="typo-t2 reviews__title js-reviews-title">Reviews</h2>

		<div class="reviews__list">

			<!-- One tile projet -->
			<div class="container">
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
			<!-- // -->

		</div>
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
