<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido(data-aos="flip-up")
      .titulo-principal__numero
        span 6
      h1 Diagrama de despliegue
    .row.mb-5
      .col-12.bg-c25
        .p-4
          .row
            .col-lg-9.order-2.order-lg-1(data-aos="fade-right")
              p Los diagramas de despliegue, que forman parte de los tipos de diagramas propuestos por UML, tienen como objetivo representar la arquitectura física del sistema, tanto en hardware como en #[i software], así como las conexiones entre ellos. Estos diagramas son de gran utilidad para el proceso de despliegue del sistema.
              p.mb-0 Los diagramas de despliegue utilizan un conjunto de elementos gráficos que tienen una representación y significado estandarizado. A continuación, se detalla cada uno de ellos:
            .col-lg-3.mb-4.mb-lg-0.order-1.order-lg-2(data-aos="fade-left")
              figure
                img(src='@/assets/curso/tema6/img1.png', style="width:350px" alt='').m-auto
    .row.justify-content-center(data-aos="fade-right")
      .col-md-8.col-lg.m-2
        .row
          .col-12.bg-c26
            .p-4
              figure
                img(src='@/assets/curso/tema6/img2.svg', style="width:85px" alt='La imagen muestra un cubo etiquetado con la palabra Nodo, que representa un elemento de un diagrama de despliegue, simbolizando un recurso de la red en la que se implementa el sistema.').m-auto
          .col-12.bg-c27
            .p-4
              p #[b Nodos]
              p.mb-0 Representa un elemento que puede ser hardware o #[i software] y se representa por un cubo.
      .col-md-8.col-lg.m-2
        .row
          .col-12.bg-c26
            .p-4
              figure
                img(src='@/assets/curso/tema6/img3.svg', style="width:300px" alt='La imagen muestra un ícono que representa un artefacto, típicamente utilizado en los diagramas de despliegue para simbolizar archivos o productos del desarrollo de software.').m-auto
          .col-12.bg-c27
            .p-4
              p #[b Artefactos]
              p.mb-0 Representan elementos concretos generados en el proceso de desarrollo, por ejemplo, bibliotecas, archivos, entre otros.
      .col-md-8.col-lg.m-2
        .row
          .col-12.bg-c26
            .p-4
              figure
                img(src='@/assets/curso/tema6/img4.svg', style="width:200px" alt='La imagen muestra dos cubos etiquetados como Nodo, con una línea que los conecta. Esto representa dos recursos de red en un diagrama de despliegue, donde la línea simboliza la comunicación o el enlace de red entre ellos.').m-auto
          .col-12.bg-c27
            .p-4
              p #[b Asociación de comunicación]
              p.mb-0 Representa el camino de comunicación entre nodos, ilustrado mediante una línea continua que une los nodos correspondientes.
    .row.justify-content-center(data-aos="fade-left")
      .col-md-8.col-lg-4.m-2
        .row
          .col-12.bg-c26
            .p-4
              figure
                img(src='@/assets/curso/tema6/img5.svg', style="width:310px" alt='La imagen muestra un cubo tridimensional etiquetado como Dispositivo. Se listan tres atributos, cada uno seguido por la palabra Tipo, y dos operaciones, cada una seguida de (lista arg) retorno.').m-auto
          .col-12.bg-c27
            .p-4
              p #[b Dispositivos]
              p.mb-0 Es un tipo especial de nodo que representa un recurso computacional del sistema, por ejemplo, un servidor.
      .col-md-8.col-lg-4.m-2
        .row
          .col-12.bg-c26
            .p-4
              figure
                img(src='@/assets/curso/tema6/img6.svg', style="width:350px" alt='La imagen representa una lista titulada Especificación de despliegue, que detalla cinco Atributos, cada uno con su respectivo tipo, como parte de un diagrama de despliegue.').m-auto
          .col-12.bg-c27
            .p-4
              p #[b Especificaciones de despliegue]
              p.mb-0 Representan configuraciones que se deben tener en cuenta para desplegar un artefacto en un nodo.

</template>

<script>
export default {
  name: 'Tema6',
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
