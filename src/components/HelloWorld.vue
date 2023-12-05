<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      - Leia mais sobre o SPIFFE
      <a href="https://spiffe.io/" target="_blank" rel="noopener">aqui</a>!
    </h3>
    <h3>
      - Visite a página do projeto no
      <a href="https://github.com/HPE-USP-SPIRE/signed-assertions" target="_blank" rel="noopener"
        >GitHub</a
      >!
    </h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
  margin-top: 1rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
