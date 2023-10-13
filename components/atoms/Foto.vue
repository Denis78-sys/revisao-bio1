<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div>
    <img class="foto" :src="require('@/assets/images/foto.jpg')" alt="Foto" />
  </div>
</template>

<style scoped>
.foto {
  width: 160px;
  border-radius: 50%;
  border: 3px solid white;
}

@media (max-width: 767px) {
    .foto{
        width: 96px;
    }
}

@media (min-width: 768px) and (max-width: 991px) {
  /* Estilos para telas de 768px a 991px de largura (geralmente smartphones em modo paisagem) */
  .foto{
        width: 104px;
    }
}
</style>
