<template>
  <div class="home-page">
    <Header />
    <Container1 class="containerInfo">
      <Informacoes class="info" />
      <AreaCta class="cta-area" />
    </Container1>
  </div>
</template>

<style scoped>
.containerInfo {
  margin-top: 32px;
}

.info{
    margin-top: 20px;
}

.cta-area {
  margin-top: 40px;
  margin-bottom: 40px;
}

@media (max-width: 767px) {
  .containerInfo {
    margin-top: 19px;
  }
  .info{
    margin-top: 16px;
}
}
</style>
