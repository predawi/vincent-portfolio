<template>
    <div class="reviews__item">
        <div class="reviews__infos">
            <img v-if="imgSrc" :src="imgSrc" :alt="imgAlt" class="reviews__avatar" />
            <div class="reviews__metas">
                <h3 v-if="author" class="reviews__author">{{ author }}</h3>
                <span v-if="company" class="typo-category reviews__category">{{ company }}</span>
            </div>
        </div>

        <div v-if="review" class="reviews__content">{{ review }}</div>

        <a v-if="link" :href="link" class="reviews__link">Voir l'avis</a>
    </div>
</template>

<script>
export default {
name: 'review-card',
props: ['imgSrc', 'imgAlt', 'author', 'company', 'review', 'link'],
}
</script>
