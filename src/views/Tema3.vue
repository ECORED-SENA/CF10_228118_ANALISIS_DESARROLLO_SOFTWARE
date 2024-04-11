<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 3
      h1 Patrones creacionales
    .row.bg-c15
      .col-12
        .px-5
          .row.mb-5
            .col-lg-8.order-2.order-lg-1
              p Una de las labores comunes en el proceso de construcción de software es precisamente distribuir responsabilidades en un conjunto de módulos o clases, siguiendo los principios definidos en los paradigmas de programación, como por ejemplo la programación orientada a objetos. Sin embargo, al momento de dar solución a un requerimiento particular se requerirá instanciar objetos de diferentes tipos, los cuales bajo sus responsabilidades implementan algún tipo de lógica.
              .row.align-items-center
                .col-auto.pe-0.d-none.d-md-block
                  figure
                    img(src='@/assets/curso/tema3/img1.svg', style="width:70px" alt='').m-auto
                .col
                  p.mb-0 En el recurso que le presentamos a continuación, profundice en los aspectos más importantes de los patrones creacionales:
            .col-lg-4.mb-4.mb-lg-0.order-1.order-lg-2
              figure
                img(src='@/assets/curso/tema3/img2.png', style="width:380px" alt='').m-auto
          figure
            .video
              iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)

</template>

<script>
export default {
  name: 'Tema3',
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
