<template>
    <section class="project-paragraph">
        <div class="container">
            <div class="typo-p project-paragraph__content" 
                v-html="htmlText" 
                :class="[isSmall ? 'project-paragraph__content--small' : '']
            ">
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'project-paragraph',
    props: ['htmlText', 'isSmall'],
}
</script>

<style lang="scss">
.project-paragraph {
    &__content {
        margin: rem(70px) 0 0;

        @include tablet {
            max-width: 584px;
            margin: rem(70px) 0 0 rem(100px);
        }

        &--small {
            @include tablet {
                max-width: 460px;
            }
        }
    }
}
</style>
