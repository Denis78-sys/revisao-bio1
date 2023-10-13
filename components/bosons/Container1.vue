<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div class="container1">
    <slot />
  </div>
</template>

<style scoped>
.container1 {
  width: 720px;
  margin: auto;
}

@media (max-width: 767px) {
  .container1 {
    width: 90%;
    margin: auto;
  }
}

@media (min-width: 768px) and (max-width: 991px) {
  /* Estilos para telas de 768px a 991px de largura (geralmente smartphones em modo paisagem) */

  .container1{
    width: 80%;
    margin: auto;
  }
}
</style>
