<template>
    <div class="projects__card">
        <NuxtLink :to="'/projects/' + link" class="projects__link">
            <div class="projects__infos">
                <h3 class="projects__title">{{ title }}</h3>
                <span v-if="category" class="typo-category projects__category">{{ category }}</span>
            </div>
        </NuxtLink>
    </div>
</template>

<script>
export default {
name: 'project-card',
props: ['link', 'title', 'category'],
}
</script>

<style lang="scss">
.projects {
    &__card {
        position: relative;
        display: flex;
        align-items: flex-end;
        justify-content: flex-end;
        height: rem(215px);
        margin-top: rem(30px);
        border: 1px solid $textcolor;
        background: $maincolor;

        @include tablet {
            height: rem(300px);
            margin-top: rem(20px);
        }
    }

    &__link {
        position: absolute;
        top: 0;
        left: 0;
        display: flex;
        align-items: flex-end;
        justify-content: flex-end;
        width: 100%;
        height: 100%;
        padding: rem(30px);
    }

    &__infos {
        text-align: right;
    }

    &__title {
        margin: 0;
        line-height: rem(28px);
        font-size: rem(24px);
        font-weight: 300;
        @extend %fontCanela;
    }

    &__category {
        display: block;
        margin-top: rem(10px);
        text-transform: uppercase;
        font-size: rem(12px);
        letter-spacing: 0.07em;
        @extend %fontManrope;
    }
}
</style>
