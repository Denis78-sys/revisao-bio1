<!-- eslint-disable vue/multi-word-component-names -->
<template>
    <div class="informacoes">
        <AreaLogoRedes class="logo-redes"/>
        <Descricao />
    </div>
</template>

<style scoped>
.logo-redes{
    margin-bottom: 16px;
}

@media (max-width: 767px) {
    .logo-redes{
        margin-bottom: 28px;
    }
}
</style>