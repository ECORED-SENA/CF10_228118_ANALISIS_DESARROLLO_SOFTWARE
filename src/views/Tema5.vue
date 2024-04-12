<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido(data-aos="flip-up")
      .titulo-principal__numero
        span 5
      h1 Vistas estáticas
    .row.align-items-center.mb-5
      .col-lg-10.order-2.order-lg-1(data-aos="fade-right")
        p La vista estática está encargada de modelar los conceptos significativos del dominio de la aplicación desde sus propiedades internas y las relaciones existentes. Se denomina vista estática porque no modela el comportamiento del sistema ni muestra las variaciones que se puedan presentar por efecto del tiempo.
        p.mb-0 Los elementos fundamentales de la vista estática son las clases que describen los conceptos del dominio del problema y las relaciones que pueden ser de tipo:
      .col-lg-2.mb-4.mb-lg-0.order-1.order-lg-2(data-aos="fade-left")
        figure
          img(src='@/assets/curso/tema4/img3.svg', style="width:180px" alt='').m-auto
    .row.justify-content-center.mb-5
      .col-10.bg-c24(data-aos="fade-down")
        .p-4
          figure.d-none.d-lg-block
            img(src='@/assets/curso/tema5/img1.svg', style="width:750px" alt='Los elementos fundamentales de la vista estática son las clases que describen los conceptos del dominio del problema y las relaciones que pueden ser de tipo: asociación, dependencia y generalización.').m-auto
          figure.d-block.d-lg-none
            img(src='@/assets/curso/tema5/img1m.svg', style="width:250px" alt='Los elementos fundamentales de la vista estática son las clases que describen los conceptos del dominio del problema y las relaciones que pueden ser de tipo: asociación, dependencia y generalización.').m-auto
    .row
      .col-lg-4.mb-4.mb-lg-0(data-aos="fade-right")
        figure
          img(src='@/assets/curso/tema5/img1.png', style="width:350px" alt='').m-auto
      .col-lg-8(data-aos="fade-left")
        p Entre los diagramas de Lenguaje Unificado de Modelado (UML) que se utilizan para representar la vista estática del sistema encontramos (ITCA, 2021):
        ul.lista-ul.mb-0
          li.d-flex
            i.fas.fa-code(style="color: #1682FB")
            |
            p.mb-0 #[b Diagrama de clases.]
          li.d-flex
            i.fas.fa-code(style="color: #1682FB")
            |
            p.mb-0 #[b Diagrama de objetos.]
          li.d-flex
            i.fas.fa-code(style="color: #1682FB")
            |
            p.mb-0 #[b Diagramas de componentes.]

</template>

<script>
export default {
  name: 'Tema5',
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
