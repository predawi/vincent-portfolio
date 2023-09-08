<template>
	<section class="projects">
		<div class="container">
			<h2 class="typo-t2 projects__title">Latest works</h2>

			<p class="typo-p">I’ve been creating digital products and experiences for more than 7 years in freelance. I had the chance to work for a lot of different industries and companies</p>
		</div>

		<div class="projects__list">

			<!-- One tile projet -->
			<div class="container">
				<project-card link="anoti" title="Anoti" category="SAAS COMPLIANCE" />
			</div>
			
			<!-- Three tiles projects -->
			<div class="projects__row">
				<project-card link="anoti" title="BNP Paribas" category="SAAS COMPLIANCE" />
				<project-card link="anoti" title="BNP Paribas" category="SAAS COMPLIANCE" />
				<project-card link="anoti" title="BNP Paribas" category="SAAS COMPLIANCE" />
			</div>

			<!-- One tile projet -->
			<div class="container">
				<project-card link="anoti" title="BNP Paribas" category="SAAS COMPLIANCE" />
			</div>

		</div>
	</section>
</template>

<script>
import ProjectCard from '~/components/ProjectCard.vue'

export default {
	name: 'NuxtProjects',
	components: {
		ProjectCard,
  	},
}
</script>

<style lang="scss">
.projects {
    margin-top: rem(70px);
    overflow: hidden;

    @include tablet {
        margin-top: rem(130px);
    }

    &__title {
        margin-bottom: rem(50px);
    }

    &__row {
        display: flex;
        width: 100%;
        overflow: scroll;

        @include tablet {
            max-width: 900px;
            margin: auto;
        }

        .projects__card {
            width: rem(324px);
            flex: 0 0 rem(324px);
            margin-left: rem(30px);

            @include tablet {
                flex: 0 1 34%;
                margin-left: 0;
            }

            &:first-of-type {
                margin-left: rem(25px);

                @include tablet {
                    margin-left: 0;
                    border-right: 0;
                }
            }

            &:last-of-type {
                margin-right: rem(25px);

                @include tablet {
                    margin-right: 0;
                    border-left: 0;
                }
            }
        }
    }

    &__list {
        margin-top: rem(50px);

        @include tablet {
            margin-top: rem(90px);
        }
    }
}
</style>

