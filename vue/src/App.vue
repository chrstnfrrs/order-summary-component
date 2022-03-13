<template>
  <div class="app-layout">
    <OrderSummary />
  </div>
</template>

<script>
import OrderSummary from "./components/OrderSummary.vue";

export default {
  name: "App",
  components: {
    OrderSummary,
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Red+Hat+Display:wght@400;500;700;900&display=swap");

html {
  font-family: "Red Hat Display", Helvetica, Arial, sans-serif;
  src: local("Red Hat Display"), local("Red Hat Display"),
    url(https://fonts.googleapis.com/css2?family=Red+Hat+Display:wght@400;500;700;900)
      format("woff2");
  font-display: swap;
}

* {
  box-sizing: border-box;
}

body,
p {
  margin: 0;
}

figure {
  display: flex;
  margin: 0;
}

img {
  height: 100%;
  width: 100%;
}

:root {
  --very-pale-blue: hsl(225, 100%, 98%);
  --desaturated-blue: hsl(224, 23%, 55%);
  --dark-blue: hsl(223, 47%, 23%);
  --bright-blue: hsl(245, 75%, 52%);
  --white: #fff;
}

#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #E0E8FF;
  background-image: url(./assets/pattern-background-desktop.svg);
  background-repeat: no-repeat;
  background-size: contain;
  @media only screen and (max-width: 660px) {
    background-image: url(./assets/pattern-background-mobile.svg);
  }
}

.app-layout {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  min-width: 100vw;
  padding: 1.5rem;
}
</style>
