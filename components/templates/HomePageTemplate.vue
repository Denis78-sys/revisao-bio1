<template>
  <div class="home-page">
    <Header />
    <div class="containerInfo">
      <Informacoes />
      <AreaCta />
    </div>
  </div>
</template>

<style scoped>
.containerInfo{
  width: 60%;
  margin: auto;
}
@media (max-width: 767px) {
  .containerInfo {
    margin-top: 19px;
    width: 90%;
  }
  
}
</style>
