<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 2
      h1 Patrones comportamentales
    p.mb-5 Los patrones de diseño comportamentales se centran en definir la manera en que los objetos interactúan entre ellos, por medio de mensajes. Son tres los tipos de patrones comportamentales: estrategia, comando e iterador.
    .row.bg-c10.mb-5
      .col-12
        .px-5
          .row.mb-4
            .col-auto.bg-c9
              .px-3.pb-0
                .row.align-items-end
                  .col-auto.px-0
                    figure.fig-p1
                      img(src='@/assets/curso/tema2/img1.svg', style="width:50px" alt='').m-auto
                  .col
                    h3.text-white Estrategia
          .row.align-items-center.mb-5
            .col-lg-8.order-2.order-lg-1
              p El patrón estrategia permite encapsular un conjunto de algoritmos de manera que puedan ser seleccionados dinámicamente para su ejecución, durante el tiempo de ejecución y de acuerdo con las acciones del cliente. Este patrón es una de las formas en las que se ven reflejadas fácilmente, las características de la programación orientada a objetos, particularmente en lo referente a encapsulamiento y polimorfismo. Landa. (2018).
              p.mb-0 Este patrón de diseño es útil cuando una misma funcionalidad puede ser provista usando diferentes mecanismos, algoritmos o estrategias, que serán seleccionadas dependiendo de las acciones realizadas por el cliente, en el momento que está ejecutando el programa.
            .col-lg-4.mb-4.mb-lg-0.order-1.order-lg-2
              figure
                img(src='@/assets/curso/tema2/img1.png', style="width:370px" alt='').m-auto
          .row.justify-content-center
            .col-lg-10.bg-c11
              .p-4
                p #[b Ejemplo]
                p.mb-5 Suponga que quiere implementar una calculadora, la cual provee un conjunto de operaciones (suma, resta, multiplicación y división) que serán usadas por el cliente según su deseo. Cada una de estas operaciones representan una estrategia diferente y será el cliente quien invocará la ejecución de cada una de ellas dependiendo de su deseo por medio de una interfaz que, usando las propiedades del polimorfismo, se transformará para poder responder a cada solicitud.
                figure.d-none.d-lg-block
                  img(src='@/assets/curso/tema2/img3.svg', style="width:650px" alt='').m-auto
                figure.d-block.d-lg-none
                  img(src='@/assets/curso/tema2/img3m.svg', style="width:450px" alt='').m-auto
    .row.bg-c10.mb-5
      .col-12
        .px-5
          .row.mb-4
            .col-auto.bg-c9
              .px-3.pb-0
                .row.align-items-end
                  .col-auto.px-0
                    figure.fig-p1
                      img(src='@/assets/curso/tema2/img1.svg', style="width:50px" alt='').m-auto
                  .col
                    h3.text-white Comando
          p.mb-5 El patrón comando permite aislar los objetos que realizan una petición de los objetos concretos encargados de recibir y realizar dicha acción, esto permite entre otras cosas, que las peticiones puedan ser enviadas a varios receptores y si se maneja el estado de las solicitudes, controla acciones de tipo Undo y Redo. El patrón comando necesita la implementación de varios elementos:
          .row.justify-content-center.mb-4
            .col-10.col-md-4.col-lg.m-2
              .row
                .col-12.bg-c12
                  .p-1
                    p.text-white.text-center.mb-0 #[b Comando]
                .col-12.bg-c13
                  .p-1
                    p.text-center.mb-0 #[b Clase que sirve de puente entre el cliente y los receptores.]
            .col-10.col-md-4.col-lg.m-2
              .row
                .col-12.bg-c12
                  .p-1
                    p.text-white.text-center.mb-0 #[b #[i Invoker]]
                .col-12.bg-c13
                  .p-1
                    p.text-center.mb-0 #[b Elemento usado por los clientes y que le solicita al comando llevar a cabo una acción.]
            .col-10.col-md-4.col-lg.m-2
              .row
                .col-12.bg-c12
                  .p-1
                    p.text-white.text-center.mb-0 #[b Cliente]
                .col-12.bg-c13
                  .p-1
                    p.text-center.mb-0 #[b Invoca la ejecución de las acciones desde el #[i Invoker].]
            .col-10.col-md-4.col-lg.m-2
              .row
                .col-12.bg-c12
                  .p-1
                    p.text-white.text-center.mb-0 #[b Icomando]
                .col-12.bg-c13
                  .p-1
                    p.text-center.mb-0 #[b Interfaz donde se especifican las operaciones a ejecutar.]
            .col-10.col-md-4.col-lg.m-2
              .row
                .col-12.bg-c12
                  .p-1
                    p.text-white.text-center.mb-0 #[b Receptor]
                .col-12.bg-c13
                  .p-1
                    p.text-center.mb-0 #[b Clase que realiza la acción.]
            .col-10.col-md-4.col-lg.m-2
              .row
                .col-12.bg-c12
                  .p-1
                    p.text-white.text-center.mb-0 #[b Ejecutar]
                .col-12.bg-c13
                  .p-1
                    p.text-center.mb-0 #[b Operación que necesita ser llevada a cabo.]
          .row.justify-content-center
            .col-lg-10.bg-c11
              .p-4
                p #[b Ejemplo]
                p.mb-5 Una persona (#[b Cliente]) quiere hacer uso del televisor y hace todas las solicitudes de servicios por medio del control remoto (#[b #[i Invoker]]). El control remoto se comunica con una interfaz encargada de responder solicitudes de cada comando, que el usuario puede hacer como, por ejemplo, prender el televisor, apagar el televisor, subir el volumen, entre otros. Cada comando realiza una acción particular sobre el televisor (#[b Receptor]).
                figure.d-none.d-lg-block
                  img(src='@/assets/curso/tema2/img4.svg', style="width:380px" alt='').m-auto
                figure.d-block.d-lg-none
                  img(src='@/assets/curso/tema2/img4m.svg', style="width:300px" alt='').m-auto
    .row.bg-c10.mb-4
      .col-12
        .px-5
          .row.mb-4
            .col-auto.bg-c9
              .px-3.pb-0
                .row.align-items-end
                  .col-auto.px-0
                    figure.fig-p1
                      img(src='@/assets/curso/tema2/img1.svg', style="width:50px" alt='').m-auto
                  .col
                    h3.text-white Iterador
          .row.align-items-center.mb-5
            .col-lg-8.order-2.order-lg-1
              p Este patrón de diseño está orientado al trabajo con colecciones y facilita el acceso a todos los elementos de la colección sin tener la necesidad de conocer su estructura.
              p.mb-0 En este patrón se reconocen los enumeradores y los iteradores. Los enumeradores se establecen para conocer el siguiente elemento de la estructura y los iteradores corresponden a un mecanismo para recorrer la estructura, de acuerdo con su secuencia, de inicio a fin. El enumerado se encarga de implementar un conjunto de métodos estándar para poder establecer la secuencia con la que se debe recorrer la estructura.
            .col-lg-4.mb-4.mb-lg-0.order-1.order-lg-2
              figure
                img(src='@/assets/curso/tema2/img2.png', style="width:370px" alt='').m-auto
          .row
            .col-12.bg-c14
              .p-4
                .row
                  .col-lg-3.mb-4.mb-lg-0
                    figure
                      img(src='@/assets/curso/tema2/img5.svg', style="width:270px" alt='').m-auto
                  .col-lg-9
                    p Los métodos más comunes:
                    ul.lista-ul.mb-0
                      li.d-flex
                        i.fas.fa-code(style="color: #1682FB")
                        |
                        p.mb-0 #[b #[i MoveNext()]] que indica si existe o no un próximo elemento por recorrer.
                      li.d-flex
                        i.fas.fa-code(style="color: #1682FB")
                        |
                        p.mb-0 #[b #[i Método Current()]] que devuelve el valor actual de la colección según la posición actual en la secuencia.
                      li.d-flex
                        i.fas.fa-code(style="color: #1682FB")
                        |
                        p.mb-0 #[b #[i Método Reset()]] que permite iniciar nuevamente la secuencia a su punto de partida.
    p.mb-5 El iterador necesita del enumerador para poder hacer el proceso de recorrido. Este tipo de operaciones son tan comunes en los sistemas actuales, que los lenguajes de programación ya poseen una implementación propia del patrón iterador.
    .row.bg-c15
      .col-12
        .px-5
          .row.justify-content-center.mb-5
            .col-lg-10
              .titulo-sexto.color-acento-contenido
                p.mb-0 #[b Figura 1.] Ejemplo para el patrón comportamental iterador
              figure.d-none.d-lg-block
                  img(src='@/assets/curso/tema2/img7.svg', style="width:1050px" alt='').m-auto
              figure.d-block.d-lg-none
                img(src='@/assets/curso/tema2/img7m.svg', style="width:300px" alt='').m-auto

</template>

<script>
export default {
  name: 'Tema2',
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
