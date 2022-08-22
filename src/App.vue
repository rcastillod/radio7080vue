<template>
  <div id="app">
    <Header/>
    <!-- <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </nav> -->
    <router-view/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
  
  export default {
    components: {
      Header,
    },  
  }
</script>

<style lang="scss">
/* -------------------------------------------------------------------------- */
/*                              CUSTOM PROPERTIES                             */
/* -------------------------------------------------------------------------- */

:root {
  --color-primary: hsl(36, 100%, 53%);
  --color-dark: hsl(0deg 0% 0%);
  --color-light: hsl(0deg 100% 100%);

  --ff-body: 'Dosis', sans-serif;

  --fw-ligth: 200;
  --fw-regular: 500;
  --fw-bold: 600;
}

/* -------------------------------------------------------------------------- */
/*                                    RESET                                   */
/* -------------------------------------------------------------------------- */
/* Box sizing rules */
*,
*::before,
*::after {
  box-sizing: border-box;
}

/* Remove default margin */
* {
  font-family: inherit;
  margin: 0;
  padding: 0;
}

/* Remove list styles on ul, ol elements with a list role, which suggests default styling will be removed */
ul[role='list'],
ol[role='list'] {
  list-style: none;
}

/* Set core root defaults */
html:focus-within {
  scroll-behavior: smooth;
}

html,
body {
  height: 100%;
}

/* Set core body defaults */
body {
  text-rendering: optimizeSpeed;
  line-height: 1.5;
}

/* A elements that don't have a class get default styles */
a:not([class]) {
  text-decoration-skip-ink: auto;
}

/* Make images easier to work with */
img,
picture {
  max-width: 100%;
  display: block;
}

/* Inherit fonts for inputs and buttons */
input,
button,
textarea,
select {
  font: inherit;
}

/* Remove all animations, transitions and smooth scroll for people that prefer not to see them */
@media (prefers-reduced-motion: reduce) {
  html:focus-within {
    scroll-behavior: auto;
  }
  
  *,
  *::before,
  *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
    scroll-behavior: auto !important;
  }
}

/* -------------------------------------------------------------------------- */
/*                                   GLOBAL                                   */
/* -------------------------------------------------------------------------- */
body {
  font-family: var(--ff-body);
  font-weight: var(--fw-ligth);
}
</style>
