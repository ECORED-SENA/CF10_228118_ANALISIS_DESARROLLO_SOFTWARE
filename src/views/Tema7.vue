<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido(data-aos="flip-up")
      .titulo-principal__numero
        span 7
      h1 Diagrama de componentes
    .row.mb-5
      .col-lg-3.pe-0.d-none.d-lg-block(data-aos="fade-right")
        figure
          img(src='@/assets/curso/tema7/img1.png', style="width:350px" alt='').m-auto
      .col.bg-c28(data-aos="fade-left")
        .p-4
          p.mb-0 El diagrama de componentes, uno de los diagramas sugeridos por UML, muestra una perspectiva estática del sistema de información y pertenece a los diagramas estructurales. Representa cómo se organiza y se relaciona el #[i software] en términos de componentes lógicos o físicos, como bibliotecas, módulos, paquetes y capas. Ofrece una visión general de los componentes del sistema, resaltando la organización y dependencia entre ellos, lo cual es fundamental para comprender cómo se integran y cooperan para realizar las funcionalidades del sistema.
    p.mb-5(data-aos="fade-right") Le invitamos a revisar los aspectos más característicos e importantes de los diagramas de componentes, explorando el recurso que se muestra a continuación:
    figure(data-aos="fade-left")
      .video
        iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)

</template>

<script>
export default {
  name: 'Tema7',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
