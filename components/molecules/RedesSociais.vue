<!-- eslint-disable vue/no-template-shadow -->
<template>
  <div>
    <ul class="redes-sociais">
      <li v-for="rede in redes" :key="rede.id">
        <RedeSocial :url="rede.link" :titulo="rede.nome" :logo="rede.icone" />
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      redes: [
        { id: 1, nome: "Instagram", icone: "instagram.svg", link: "https://www.instagram.com/" },
        { id: 2, nome: "Facebook", icone: "facebook.svg", link: "https://www.facebook.com/?locale=pt_BR" },
        { id: 3, nome: "Linkedin", icone: "linkedin.svg", link: "https://br.linkedin.com/" },
        { id: 4, nome: "GitHub", icone: "github.svg", link: "https://github.com/" },
        
      ],
    };
  },
};
</script>

<style scoped>
li {
  list-style: none;
}
.redes-sociais {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-gap: 8px;
  align-items: end;
}

@media (max-width: 767px) {
  .redes-sociais {
    grid-gap: 4px;
  }
}
</style>
