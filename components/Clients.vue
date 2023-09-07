<template>
	<section class="clients">
		<div class="container">
			
            <div class="clients__wrapper">
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 483 663" fill="none" class="clients__gate reveal">
                    <path class="union-path" stroke="#222" stroke-width=".5" fill="none" d="M242 1.5C110.061 1.5 3.04 108.188 2.502 240h28c.54-116.349 95.249-210.5 211.998-210.5S453.958 123.651 454.498 240h27C480.959 108.188 373.939 1.5 242 1.5ZM454.5 241h-.001l-.498 421h27l.498-421H454.5Zm-1.001-.502L453.001 662l-.001 1h29l.499-422h.001l-.001-.526.001-.474h-.002C481.959 107.635 374.491.5 242 .5 109.509.5 2.04 107.635 1.502 240l-.001.417L1.5 241 1 661.999.999 663H32L32 661.999 31.5 241m421.999-.502C453.228 124.474 358.865 30.5 242.5 30.5c-116.533 0-211 94.245-211 210.499m-1 .001h-28l-.499 420L2 662h29l-.001-1-.499-420Z" clip-rule="evenodd"/>
                </svg>

                <div class="clients__content">
                    <h2 class="clients__title">I’ve also worked with</h2>

                    <p class="clients__list">Gucci . COTY . RATP . Poilane . Open class room . Les fruits & légumes frais . FlexFuel . NOOZ . Anoti . RX Production . UX Republic . BeAPI . DVTK . Upscape . Malherbe . Retrofutur . Crédit Agricole . Plan NET . La Netscouade . Cowash . Hermès . 34 Studio . Printemps</p>
                </div>
            </div>
		</div>
	</section>
</template>

<script>
export default {
	name: 'NuxtProjects'
}
</script>

<style lang="scss">
.clients {
    margin-top: 112px;

    @include tablet {
        margin-top: 230px;
    }

    &__wrapper {
        position: relative;
        max-width: 480px;
        margin: auto;
    }

    &__gate {
        display: block;
        width: 100%;
    }

    &__content {
        position: absolute;
        top: 0;
        left: 0;
        display: flex;
        flex-flow: column;
        justify-content: flex-end;
        width: 100%;
        height: 100%;
        padding: 0 rem(40px);

        @include tablet {
            padding: 0 rem(85px);
        }
    }

    &__title {
        margin: 0;
        line-height: rem(74px);
        font-size: rem(70px);
        font-weight: 100;
        letter-spacing: -0.04em;
        text-align: center;
        @extend %fontCanela;

        @include tablet {
            line-height: rem(99px);
            font-size: rem(97px);
        }
    }

    &__list {
        margin: rem(30px) 0 0;

        @include tablet {
            margin: rem(47px) 0 0;
        }
    }
}
</style>
