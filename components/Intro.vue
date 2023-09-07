<template>
    <section class="intro">
        <div class="container">
            <h1 class="typo-t1 intro__title">Experience <br>designer</h1>

            <p class="typo-p">I am a freelance senior product designer. I help companies and agencies worldwide to think, design and create innovative digital and phygital experiences</p>

            <p class="typo-p">I’m aiming to build meaningful user and customer experiences which explore the endless creative possibilities that a digital medium offers. I enjoy working on finding the perfect combination of Creativity, Strategy & Experience</p>

            <NuxtLink to="/about" class="typo-link intro__link">Find out more</NuxtLink>
        </div>
    </section>
</template>

<style lang="scss">
.intro {
    margin-top: rem(30px);

    @include tablet {
        margin-top: rem(150px);
    }

    &__title {
        @include tablet {
            margin-bottom: rem(50px);
        }
    }

    &__link {
        display: inline-block;

        @include tablet {
            margin-top: rem(50px);
        }
    }
}
</style>
