<template lang="pug">
.curso-main-container.introduccion
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido(data-aos="flip-up")
      .titulo-principal__numero
        span
          i.fas.fa-info
      h1 Introducción
    .row.bg-c1
      .col-12
        .px-5
          .row.align-items-center.mb-5
            .col-lg-3.mb-4.mb-lg-0(data-aos="fade-right")
              figure
                img(src='@/assets/curso/intro/img1.png', style="width:400px" alt='').m-auto
            .col-lg-9(data-aos="fade-left")
              p Los patrones de diseño surgen, inicialmente, en el área de la arquitectura y la ingeniería civil, refiriéndose a casos particulares a los que se enfrentaron en algún momento y de los cuales se documentó una solución particular. Posteriormente, este concepto se empezó a asociar al diseño orientado a objetos. En lugar de referirse a la forma de colocar paredes, puertas y ventanas, se hizo referencia a la forma en que se construyen clases, objetos e interfaces, y la forma en cómo estos deben interactuar.
              .row
                .col-12.bg-c2
                  .p-4
                    .row.align-items-center
                      .col-md-auto.mb-4.mb-md-0
                        figure
                          img(src='@/assets/curso/intro/img1.svg', style="width:70px" alt='').m-auto
                      .col
                        p.mb-0 Los patrones de diseño del #[i software] representan un conjunto de formas estandarizadas para resolver un problema particular, los cuales surgen a partir de la experiencia desarrollada en la industria.
          p.mb-4(data-aos="fade-right") Un patrón de diseño debe estar estructurado por cuatro componentes:
          .row.align-items-center.mb-5
            .col-lg-8.order-2.order-lg-1(data-aos="fade-right")
              .row.mb-3
                .col-12
                  .row.justify-content-center
                    .col-10.col-md-5.col-lg.bg-c3.m-2
                      .p-3
                        figure.mb-3
                          img(src='@/assets/curso/intro/img2.svg', style="width:110px" alt='').m-auto
                        p.text-white.text-center.mb-0 El nombre.
                    .col-10.col-md-5.col-lg.bg-c3.m-2
                      .p-3
                        figure.mb-3
                          img(src='@/assets/curso/intro/img3.svg', style="width:70px" alt='').m-auto
                        p.text-white.text-center.mb-0 Problema o contexto de aplicación.
                    .col-10.col-md-5.col-lg.bg-c3.m-2
                      .p-3
                        figure.mb-3
                          img(src='@/assets/curso/intro/img4.svg', style="width:70px" alt='').m-auto
                        p.text-white.text-center.mb-0 Solución propuesta.
                    .col-10.col-md-5.col-lg.bg-c3.m-2
                      .p-3
                        figure.mb-3
                          img(src='@/assets/curso/intro/img5.svg', style="width:70px" alt='').m-auto
                        p.text-white.text-center.mb-0 Ventajas y desventajas.
              p.mb-0 En este componente formativo, se abordarán algunos de los patrones de diseño más representativos en la industria del #[i software], los cuales le permitirán implementar, a futuro, soluciones más robustas acordes con los altos estándares de calidad ampliamente conocidos en la industria. Este estudio profundizará en cómo estos patrones facilitan la reutilización de soluciones probadas y eficientes, mejorando así la mantenibilidad y la escalabilidad del #[i software].
            .col-lg-4.mb-4.mb-lg-0.order-1.order-lg-2(data-aos="fade-left")
              figure
                img(src='@/assets/curso/intro/img2.png', style="width:400px" alt='').m-auto
    
</template>

<script>
export default {
  name: 'Introduccion',
  data: () => ({
    // variables de vue
  }),
}
</script>

<style lang="sass"></style>
