<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido(data-aos="flip-up")
      .titulo-principal__numero
        span 4
      h1 Patrones estructurales
    p.mb-4(data-aos="fade-right") Los patrones estructurales proveen una orientación relacionada con la forma de definir los componentes de los objetos. Dentro de los patrones estructurales se encuentran:
    .row.align-items-center
      .col-lg-9.order-2.order-lg-1(data-aos="fade-right")
        .row
          .col-12.bg-c4
            .p-2
              .row.align-items-center
                .col-md-auto.mb-3.mb-md-0
                  figure
                    img(src='@/assets/curso/tema4/img1.svg', style="width:70px" alt='').m-auto
                .col
                  p.mb-0 #[b El patrón Fachada]
                  p.mb-0 Utilizado cuando el sistema está compuesto por varios subsistemas.
          .col-12.bg-c7
            .p-2
              .row.align-items-center
                .col-md-auto.mb-3.mb-md-0
                  figure
                    img(src='@/assets/curso/tema4/img2.svg', style="width:70px" alt='').m-auto
                .col
                  p.mb-0 #[b El patrón #[i Delegate]]
                  p.mb-0 Usado cuando se quiere reutilizar y extender funcionalidades de una clase, sin hacer uso de la herencia.
      .col-lg-3.mb-4.mb-lg-0.order-1.order-lg-2(data-aos="fade-left")
        figure
          img(src='@/assets/curso/tema4/img1.png', style="width:340px" alt='').m-auto
    Separador
    #t_4_1
    .titulo-segundo.color-acento-contenido
      h2 4.1 Fachada
    .row.bg-c16.mb-5
      .col-12
        .px-5
          .row.align-items-center.mb-5
            .col-lg-10.order-2.order-lg-1(data-aos="fade-right")
              p El patrón fachada se emplea cuando un sistema está conformado por múltiples subsistemas, lo que complica la gestión de las interacciones que el cliente debe realizar con cada uno de ellos. Este patrón permite generar al cliente una vista de alto nivel que simplifica el control y el envío de mensajes a los subsistemas, ocultando los detalles relacionados con la gestión de las clases e instancias.
              p.mb-0 Existen diferentes variaciones del patrón fachada:
            .col-lg-2.mb-4.mb-lg-0.order-1.order-lg-2(data-aos="fade-left")
              figure
                img(src='@/assets/curso/tema4/img3.svg', style="width:180px" alt='').m-auto
          .row.justify-content-center.mb-0.mb-lg-5(data-aos="fade-down")
            .col-md-6.col-lg.mb-5.mb-lg-0
              .tarjeta-avatar
                img(src='@/assets/curso/tema4/img4.svg' alt='AvatarTop')
                .tarjeta.color-primario
                  .p-4
                    p.text-center #[b Opaco]
                    p.text-center.mb-0 Una de las variaciones más utilizadas y en la cual los clientes no pueden acceder a los subsistemas, solo se puede hacer mediante el objeto fachada.
            .col-md-6.col-lg.mb-5.mb-lg-0
              .tarjeta-avatar
                img(src='@/assets/curso/tema4/img5.svg' alt='AvatarTop')
                .tarjeta.color-primario
                  .p-4
                    p.text-center #[b Transparente]
                    p.text-center.mb-0 El cliente tiene la posibilidad de acceder a los subsistemas por medio de la fachada, pero también puede hacerlo de forma directa.
            .col-md-6.col-lg.mb-5.mb-lg-0
              .tarjeta-avatar
                img(src='@/assets/curso/tema4/img6.svg' alt='AvatarTop')
                .tarjeta.color-primario
                  .p-4
                    p.text-center #[b Estática]
                    p.text-center.mb-0 En esta variación la fachada se implementa como una clase estática, por lo cual, no se hace necesaria la instancia de un objeto concreto de la fachada.
          p.mb-5(data-aos="fade-right") En este patrón se reconocen tres partes fundamentales. Landa, (2018):
          .row.justify-content-center.mb-5
            .col-lg-10(data-aos="fade-down")
              .row.align-items-center.justify-content-center.mb-4
                .col-auto.mb-2.mb-lg-0
                  figure
                    img(src='@/assets/curso/tema4/img7.svg', style="width:180px" alt='Fachada').m-auto
                .col.bg-c17
                  .p-4
                    p.mb-0 Clase que provee las operaciones de alto nivel que serán usadas por el cliente.
              .row.align-items-center.justify-content-center.mb-4
                .col-auto.mb-2.mb-lg-0
                  figure
                    img(src='@/assets/curso/tema4/img8.svg', style="width:180px" alt='Subsistemas').m-auto
                .col.bg-c17
                  .p-4
                    p.mb-0 Clases que proveen las funcionalidades que son expuestas por la fachada.
              .row.align-items-center.justify-content-center.mb-0
                .col-auto.mb-2.mb-lg-0
                  figure
                    img(src='@/assets/curso/tema4/img9.svg', style="width:180px" alt='Cliente').m-auto
                .col.bg-c17
                  .p-4
                    p.mb-0 Hace uso de las operaciones de alto nivel por medio de la fachada.
    p.mb-5(data-aos="fade-right") Se representa de la siguiente manera:
    .row.justify-content-center.mb-5
      .col-lg-10.bg-c18(data-aos="fade-left")
        .p-4
          .titulo-sexto.color-acento-contenido
            p.mb-0 #[b Figura 2.] Diagrama patrón fachada
          figure.d-none.d-lg-block
              img(src='@/assets/curso/tema4/img10.svg', style="width:750px" alt='La figura presenta un patrón de diseño Fachada donde un cliente interactúa con una fachada que ofrece tres operaciones. La fachada oculta la complejidad y dirige estas operaciones hacia tres subsistemas subyacentes, simplificando la interacción del cliente con el sistema.').m-auto
          figure.d-block.d-lg-none
            img(src='@/assets/curso/tema4/img10m.svg', style="width:200px" alt='La figura presenta un patrón de diseño Fachada donde un cliente interactúa con una fachada que ofrece tres operaciones. La fachada oculta la complejidad y dirige estas operaciones hacia tres subsistemas subyacentes, simplificando la interacción del cliente con el sistema.').m-auto
    p.mb-5(data-aos="fade-right") A continuación, se muestra una implementación en código Java de cada uno de los elementos requeridos para la implementación del patrón fachada en un ejemplo sencillo.
    .row.justify-content-center.mb-5.mb-lg-3
      .col-10.bg-c14
        .p-4
          .row
            .col-lg-8.order-2.order-lg-1(data-aos="fade-right")
              p #[b Ejemplo:] el cliente quiere realizar una compra, pero este proceso involucra acciones por parte de tres diferentes subsistemas:
              ul.lista-ul.mb-0
                li.d-flex
                  i.fas.fa-code(style="color: #1682FB")
                  |
                  p.mb-0 #[b Subsistema de compras:] verifica la viabilidad de la tarjeta para el pago.
                li.d-flex
                  i.fas.fa-code(style="color: #1682FB")
                  |
                  p.mb-0 #[b Subsistema de inventario:] verifica si hay productos en #[i stock].
                li.d-flex
                  i.fas.fa-code(style="color: #1682FB")
                  |
                  p.mb-0 #[b Subsistema de envíos].
            .col-lg-4.mb-4.mb-lg-0.order-1.order-lg-2(data-aos="fade-left")
              figure
                img(src='@/assets/curso/tema4/img3.png', style="width:270px" alt='').m-auto
    p.mb-5(data-aos="fade-right") Para disminuir la complejidad, de la cual no debería ocuparse el cliente, se creará una fachada que encapsula las acciones de todos los subsistemas involucrados y proveer una interfaz simple con la que el cliente podrá interactuar más fácilmente, como se presenta a continuación:
    .row.bg-c19
      .col-12
        .px-5
          .row.justify-content-center
            .col-lg-7.mb-5(data-aos="fade-right")
              p #[b Clase que representa el subsistema de compras]
              .row
                .col-12.bg-c20
                  .p-2
                    figure
                      img(src='@/assets/curso/tema4/img11.svg', style="width:50px" alt='')
                .col-12.bg-c21
                  .p-2
                    pre
                      p.mb-0 public class GestorCompra {
                      p.mb-0  private Scanner in = new Scanner(System.in);
                      p.mb-0
                      p.mb-0  public boolean comprar(){
                      p.mb-0      int numero;
                      p.mb-0      System.out.println("Ingrese el número de tarjeta para realizar el pago");
                      p.mb-0      número = in.nextInt();
                      p.mb-0      if(numero == 4567){
                      p.mb-0          System.out.println("Procesando la compra");
                      p.mb-0          System.out.println("--------------------");
                      p.mb-0          System.out.println("Pago aceptado");
                      p.mb-0          return true;
                      p.mb-0      }else{
                      p.mb-0          System.out.println("Pago rechazado");
                      p.mb-0          return false;
                      p.mb-0      }
                      p.mb-0    }
                      p.mb-0  }
            .col-lg-7.mb-5(data-aos="fade-right")
              p #[b Clase que representa el subsistema de inventario]
              .row
                .col-12.bg-c20
                  .p-2
                    figure
                      img(src='@/assets/curso/tema4/img11.svg', style="width:50px" alt='')
                .col-12.bg-c21
                  .p-2
                    pre
                      p.mb-0 public class GestorInventario {
                      p.mb-0     private int stock;
                      p.mb-0     public GestorInventario() {
                      p.mb-0         this.stock = 2;
                      p.mb-0     }
                      p.mb-0     public boolean retirarStock(){
                      p.mb-0         if(stock > 0){
                      p.mb-0             System.out.println("Producto listo para envío");
                      p.mb-0             stock--;
                      p.mb-0             return true;
                      p.mb-0         }else{
                      p.mb-0             System.out.println("Producto no disponible, no hay existencias, entrega reprogramada!");
                      p.mb-0             return false;
                      p.mb-0         }
                      p.mb-0     }    
                      p.mb-0 }
            .col-lg-7.mb-5(data-aos="fade-right")
              p #[b Clase que representa el subsistema de envíos]
              .row
                .col-12.bg-c20
                  .p-2
                    figure
                      img(src='@/assets/curso/tema4/img11.svg', style="width:50px" alt='')
                .col-12.bg-c21
                  .p-2
                    pre
                      p.mb-0 public class GestorEnvio {
                      p.mb-0   public void enviarPedido(){
                      p.mb-0     System.out.println("Envio autorizado y en camino!");
                      p.mb-0   }    
                      p.mb-0 }
            .col-lg-7.mb-5(data-aos="fade-right")
              p #[b Clase que representa la fachada de todos los subsistemas]
              .row
                .col-12.bg-c20
                  .p-2
                    figure
                      img(src='@/assets/curso/tema4/img11.svg', style="width:50px" alt='')
                .col-12.bg-c21
                  .p-2
                    pre
                      p.mb-0 public class Fachada {
                      p.mb-0 
                      p.mb-0   //Instancias de los subsistemas que gestiona
                      p.mb-0   private GestorCompra compra = new GestorCompra();
                      p.mb-0   private GestorInventario inventario = new GestorInventario();
                      p.mb-0   private GestorEnvio envio = new GestorEnvio();
                      p.mb-0 
                      p.mb-0   //Metodo de alto nivel que se ofrece al cliente
                      p.mb-0   public void compra(){
                      p.mb-0     if(compra.comprar() && inventario.retirarStock()){
                      p.mb-0       envio.enviarPedido();       
                      p.mb-0     }
                      p.mb-0   }
                      p.mb-0 }
            .col-lg-7(data-aos="fade-right")
              p #[b Clase que representa al cliente]
              .row
                .col-12.bg-c20
                  .p-2
                    figure
                      img(src='@/assets/curso/tema4/img11.svg', style="width:50px" alt='')
                .col-12.bg-c21
                  .p-2
                    pre
                      p.mb-0 public class Cliente {
                      p.mb-0   public static void main(String[] args) {
                      p.mb-0     Fachada fachada = new Fachada();
                      p.mb-0     // Se hace uso de las operaciones de alto nivel
                      p.mb-0     fachada.compra();
                      p.mb-0     fachada.compra();
                      p.mb-0     fachada.compra();
                      p.mb-0   }
                      p.mb-0 }
    Separador
    #t_4_2
    .titulo-segundo.color-acento-contenido
      h2 4.2 #[i Delegate]
    .row.align-items-center.mb-5
      .col-lg-8.order-2.order-lg-1(data-aos="fade-right")
        p El patrón #[i delegate] se usa cuando se quiere reutilizar y extender funcionalidades de una clase sin hacer uso de la herencia. Este patrón permite de cierta forma implementar algo similar a la herencia múltiple que no es admitido por algunos lenguajes de programación, pero adicionalmente permite tener un control más detallado sobre este proceso, ya que se puede ocultar parte de los elementos heredados o, incluso, compartir elementos que no son posibles de heredar bajo el mecanismo de herencia tradicional.
        .row.mb-3
          .col-12.bg-c22
            .p-3
              p.mb-0 #[b Este patrón busca evitar la concentración de todas las responsabilidades en una única instancia, optando en cambio, por delegar las tareas en otras instancias especializadas en resolver dichas funciones.]
        .row.align-items-center
          .col-auto.pe-0
            figure
              img(src='@/assets/curso/tema4/img12.svg', style="width:70px" alt='').m-auto
          .col
            p.mb-0 En el siguiente ejemplo se muestra la implementación del patrón de diseño en cuestión, donde se aplica el patrón #[i Delegate] para #[b integrar en una clase concreta funcionalidades definidas en otras clases a través del uso de interfaces].
      .col-lg-4.mb-4.mb-lg-0.order-1.order-lg-2(data-aos="fade-left")
        figure
          img(src='@/assets/curso/tema4/img6.png', style="width:370px" alt='').m-auto
    .row.bg-c23
      .col-12
        .px-5
          .row.justify-content-center
            .col-lg-7.mb-5(data-aos="fade-left")
              p #[b 1. Creación de interfaces para comportamientos reutilizables]
              .row
                .col-12.bg-c20
                  .p-2
                    figure
                      img(src='@/assets/curso/tema4/img11.svg', style="width:50px" alt='')
                .col-12.bg-c21
                  .p-2
                    pre
                      p.mb-0 public interface IDisenadora {    
                      p.mb-0     void disenar();
                      p.mb-0 }
                      p.mb-0 public interface ICodificadora {
                      p.mb-0     void codificar();  
                      p.mb-0 }
            .col-lg-7.mb-5(data-aos="fade-left")
              p #[b 2. Implementación de interfaces en clases concretas]
              .row
                .col-12.bg-c20
                  .p-2
                    figure
                      img(src='@/assets/curso/tema4/img11.svg', style="width:50px" alt='')
                .col-12.bg-c21
                  .p-2
                    pre
                      p.mb-0 public class ClaseCodificadora implements ICodificadora{
                      p.mb-0    @Override
                      p.mb-0    public void codificar() {
                      p.mb-0        System.out.println("Codificación por la clase codificadora");
                      p.mb-0    } 
                      p.mb-0 }
                      p.mb-0
                      p.mb-0 public class ClaseDisenadora implements IDisenadora{
                      p.mb-0    @Override
                      p.mb-0    public void disenar() {
                      p.mb-0        System.out.println("Diseñado por clase Diseñadora");
                      p.mb-0    }  
                      p.mb-0 }
            .col-lg-7.mb-5(data-aos="fade-left")
              p #[b 3. Generación de clase reutilizadora de funcionalidades]
              .row
                .col-12.bg-c20
                  .p-2
                    figure
                      img(src='@/assets/curso/tema4/img11.svg', style="width:50px" alt='')
                .col-12.bg-c21
                  .p-2
                    pre
                      p.mb-0 public class Empleado implements ICodificadora,IDisenadora{
                      p.mb-0    ICodificadora codificador;
                      p.mb-0    IDisenadora disenador;
                      p.mb-0
                      p.mb-0    public Empleado(ICodificadora codificador, IDisenadora disenador) {
                      p.mb-0        this.codificador = codificador;
                      p.mb-0        this.disenador = disenador;
                      p.mb-0    }
                      p.mb-0    @Override
                      p.mb-0    public void codificar() {
                      p.mb-0        codificador.codificar();
                      p.mb-0    }
                      p.mb-0    @Override
                      p.mb-0    public void disenar() {
                      p.mb-0        disenador.disenar();
                      p.mb-0    }   
                      p.mb-0 }
            .col-lg-8.mb-5(data-aos="fade-left")
              p #[b 4. Instanciación de la clase principal con clases concretasrserán reutilizados]
              .row
                .col-12.bg-c20
                  .p-2
                    figure
                      img(src='@/assets/curso/tema4/img11.svg', style="width:50px" alt='')
                .col-12.bg-c21
                  .p-2
                    pre
                      p.mb-0 public class PatronDelegate {
                      p.mb-0     public static void main(String[] args) {
                      p.mb-0         Empleado objEmpleado = new Empleado(new ClaseCodificadora(),new ClaseDisenadora());
                      p.mb-0         objEmpleado.codificar();
                      p.mb-0         objEmpleado.disenar();
                      p.mb-0     }
                      p.mb-0 }
    p(data-aos="fade-right") Cualquier nueva clase concreta que implemente las interfaces originales podrán ser utilizadas por la clase Empleado para su reutilización, simplemente pasando la instancia correspondiente que implementa la nueva lógica al parámetro del constructor.

</template>

<script>
export default {
  name: 'Tema4',
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
