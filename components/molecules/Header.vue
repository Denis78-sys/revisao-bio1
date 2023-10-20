<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div class="header">
    <div class="faixa"></div>
    <div class="containerFoto">
      <Foto class="foto-perfil" />
    </div>
  </div>
</template>

<style scoped>
.containerFoto {
  width: 60%;
  margin: auto;
}
.faixa {
  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: 206px;
  background-color: #0f468c;
}

.foto-perfil {
  margin-top: -80px;
}

@media (max-width: 767px) {
  .foto-perfil {
    margin-top: -50px;
  }
  .containerFoto {
    width: 90%;
    
  }
  .faixa {
    grid-template-rows: 175px;
  }
}

@media (min-width: 768px) and (max-width: 991px) {
  /* Estilos para telas de 768px a 991px de largura (geralmente smartphones em modo paisagem) */
  .foto-perfil {
    margin-top: -50px;
  }

  .faixa {
    grid-template-rows: 180px;
  }
}

@media (min-width: 1200px) and (max-width: 1439px) {
  /* Estilos para telas de 1200px a 1439px de largura (geralmente laptops e monitores pequenos) */
  .foto-perfil {
    margin-top: -70px;
  }
  .faixa {
    grid-template-rows: 180px;
  }
}

@media (min-width: 1440px) {
  /* Estilos para telas com largura igual ou superior a 1440px (geralmente monitores maiores) */
  .foto-perfil {
    margin-top: -70px;
  }
  .faixa {
    grid-template-rows: 180px;
  }
}
</style>
