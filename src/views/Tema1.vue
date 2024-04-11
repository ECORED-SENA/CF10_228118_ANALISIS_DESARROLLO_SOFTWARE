<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 1
      h1 Conceptos sobre patrones de diseño
    p El uso de patrones de diseño en el ámbito de la industria de software implica el conocimiento y la aplicación de una serie de criterios que aportan calidad al proceso mismo y efectividad del producto logrado. En ese mismo sentido, se favorece la estandarización del código fuente de determinada aplicación, lo cual facilita su monitoreo y mantenimiento.
    p.mb-5 Los patrones de diseño tienen las siguientes características:
    .row.align-items-center.mb-5
      .col-lg-9.order-2.order-lg-1
        .row
          .col-12.bg-c4
            .p-2
              .row.align-items-center
                .col-md-auto.mb-3.mb-md-0
                  figure
                    img(src='@/assets/curso/tema1/img1.svg', style="width:70px" alt='').m-auto
                .col
                  p.mb-0 #[b 1.] Representan soluciones concretas que, aunque se representan de forma genérica, son aplicados para resolver problemas reales.
          .col-12.bg-c5
            .p-2
              .row.align-items-center
                .col-md-auto.mb-3.mb-md-0
                  figure
                    img(src='@/assets/curso/tema1/img2.svg', style="width:70px" alt='').m-auto
                .col
                  p.mb-0 #[b 2.] Son especificaciones técnicas basadas en los principios de la programación orientada a objetos y dependiendo del lenguaje de programación la forma de implementarlos puede variar.
          .col-12.bg-c6
            .p-2
              .row.align-items-center
                .col-md-auto.mb-3.mb-md-0
                  figure
                    img(src='@/assets/curso/tema1/img3.svg', style="width:70px" alt='').m-auto
                .col
                  p.mb-0 #[b 3.] Son frecuentemente utilizados ya que se construyen a partir de la experiencia acumulada en la industria del desarrollo de software.
          .col-12.bg-c5
            .p-2
              .row.align-items-center
                .col-md-auto.mb-3.mb-md-0
                  figure
                    img(src='@/assets/curso/tema1/img4.svg', style="width:70px" alt='').m-auto
                .col
                  p.mb-0 #[b 4.] Favorecen la implementación de las características de la programación orientada a objetos como la encapsulación, las jerarquías y el polimorfismo.
          .col-12.bg-c6
            .p-2
              .row.align-items-center
                .col-md-auto.mb-3.mb-md-0
                  figure
                    img(src='@/assets/curso/tema1/img5.svg', style="width:70px" alt='').m-auto
                .col
                  p.mb-0 #[b 5.] No necesariamente el uso de un patrón implica el uso de palabras claves, reservadas o de librerías especializadas.
          .col-12.bg-c7
            .p-2
              .row.align-items-center
                .col-md-auto.mb-3.mb-md-0
                  figure
                    img(src='@/assets/curso/tema1/img6.svg', style="width:70px" alt='').m-auto
                .col
                  p.mb-0 #[b 6.] Los patrones generalmente hacen referencia al uso de interfaces, clases y objetos que deben ser ajustados de acuerdo con la solución concreta a desarrollar.
      .col-lg-3.mb-4.mb-lg-0.order-1.order-lg-2
        figure
          img(src='@/assets/curso/tema1/img1.png', style="width:300px" alt='').m-auto
    p.mb-4 Para comprender mejor la organización y aplicación de los patrones de diseño en el desarrollo de software, es importante reconocer su clasificación. Estos suelen dividirse en tres grandes grupos, según su finalidad:
    .row
      .col-lg.bg-c8.m-2
        .p-4
          .row.align-items-center
            .col-auto
              figure
                img(src='@/assets/curso/tema1/img7.svg', style="width:70px" alt='').m-auto
            .col
              p.mb-0 #[b Patrones comportamentales]
      .col-lg.bg-c8.m-2
        .p-4
          .row.align-items-center
            .col-auto
              figure
                img(src='@/assets/curso/tema1/img8.svg', style="width:70px" alt='').m-auto
            .col
              p.mb-0 #[b Patrones creacionales]
      .col-lg.bg-c8.m-2
        .p-4
          .row.align-items-center
            .col-auto
              figure
                img(src='@/assets/curso/tema1/img9.svg', style="width:70px" alt='').m-auto
            .col
              p.mb-0 #[b Patrones estructurales]
      
</template>

<script>
export default {
  name: 'Tema1',
  components: {},
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
