<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <div class="fix">
    <header>
      <img
        alt="SPIFFE logo"
        class="logo"
        src="./assets/spiffe-icon-color.png"
        width="125"
        height="125"
      />

      <div class="wrapper">
        <HelloWorld msg="Ampliando a Expressividade dos Tokens SPIFFE" />
      </div>
    </header>
  </div>

  <main class="container">
    <TheWelcome />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

.container {
  padding: 3em 0rem 3rem 0rem;
}

@media (min-width: 1024px) {
  .container {
    padding: 8rem 0rem 8rem 0rem;
  }

  .container:before {
    content: ' ';
    border-left: 1px solid var(--color-border);
    position: fixed;
    left: 50%;
    bottom: 15%;
    height: 70%;
  }

  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
    position: fixed;
    width: 35%;
    height: 400px;
    top: calc(50% - 200px);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
