<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div >
    <a class="cta" :href="linkZap" target="_blank">{{tituloDescricao}}</a>
  </div>
</template>

<script>
export default {
  props: {
    // eslint-disable-next-line vue/require-prop-types
    tituloDescricao:{
      required: true
    },
    // eslint-disable-next-line vue/require-prop-types
    linkZap:{
      required: true
    }
  }
};
</script>

<style scoped>
a{
  text-decoration: none;
  color: white;
  font-size: 16px;
}
.cta{
    display: flex; /* Usar flexbox para alinhar verticalmente */
  justify-content: center; /* Centralizar horizontalmente */
  align-items: center; /* Centralizar verticalmente */
    height: 80px;
    background: #0F468C;
    width: 100%;
    text-align: center;
    border-radius: 16px;
    transition: transform 0.3s ease;
}
.cta:hover{
    transform: scale(1.1);
}


@media (max-width: 767px){
   .cta{
        height: 60px;
        border-radius: 8px;
    }
}
</style>
