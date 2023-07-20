<template>
  <div>
    <nav id="nav" :class="{'nav nav--open': isToggled, 'nav nav--close': !isToggled}">
      <div class="nav__inner">
        <div id="burger" @click="isToggled = !isToggled">
            <button class="nav__button">Menu</button>
        </div>

        <ul class="nav__list">
          <li class="nav__list-item">
            <NuxtLink to="/"><span>Home/</span><span>Work</span></NuxtLink>
          </li>
          <li class="nav__list-item">
            <NuxtLink to="/about">About</NuxtLink>
          </li>
          <li class="nav__list-item">
            <NuxtLink to="/contact">Contact</NuxtLink>
          </li>
        </ul>
      </div>
    </nav>
  </div>
</template>

<script>
  export default {
    data: function () {
      return {
        isToggled: false,
      }
    }
  };
</script>