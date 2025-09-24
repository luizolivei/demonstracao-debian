<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
})
</script>

<template>
  <div class="greetings">
    <h1 class="green">Aplicação Vue dentro do Debian via Docker</h1>
    <h3>
      Esta interface está sendo servida por um container Docker baseado em Debian, em execução no WSL2 do meu Windows 11. Tudo o que você vê aqui chega ao navegador pela porta 3000.
    </h3>
    <p>
      A ideia da demo é mostrar como o Docker simplifica a criação de ambientes Linux isolados mesmo dentro do Windows, deixando o fluxo de desenvolvimento consistente e repetível.
    </p>
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
}

.greetings h1,
.greetings h3,
.greetings p {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3,
  .greetings p {
    text-align: left;
  }
}
</style>
