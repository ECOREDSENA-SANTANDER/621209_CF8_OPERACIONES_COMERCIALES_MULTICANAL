<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5.borde-recto-abajo
      .titulo-principal.color-acento-contenido
        .titulo-principal__numero
          span 4
        h1 Normativa del recaudo de caja
      
      p.mb-4.mt-5 La necesidad de control en la recepción, custodia y despacho de bienes financieros en el #[em retail] ha llevado a la transformación de procedimientos destinados a cumplir con las normas de recaudo de caja. Esto incluye la implementación de recursos físicos, materiales y humanos para asegurar la precisión y seguridad en estas operaciones.
  
      TabsB.color-acento-contenido.mb-3
        .py-4.py-md-5(titulo="Controles de seguridad ambiental" :icono="require('@/assets/curso/temas/tema4/tab1-1.png')")
          .row.align-items-center.justify-content-center
            .col-6.col-md-4.col-lg-2.mb-4.mb-md-0
              img.p-3(src="@/assets/curso/temas/tema4/imgtab1-1.png" alt="")
            .col-sm-12.col-md-12.col-lg-8.mb-4.mb-md-0
              p Los controles de seguridad ambiental son registros procedimentales, administrativos, financieros y documentales que establecen las reglas a seguir para la protección del ambiente en el #[em retail]. 
              p Estos controles aseguran que todas las operaciones se realicen de manera sostenible y segura, minimizando el impacto ambiental.
        .py-4.py-md-5(titulo="Riesgos" :icono="require('@/assets/curso/temas/tema4/tab1-2.png')")
          .row.align-items-center.justify-content-center
            .col-6.col-md-4.col-lg-2.mb-4.mb-md-0
              img.p-3(src="@/assets/curso/temas/tema4/imgtab1-2.png" alt="")
            .col-sm-12.col-md-12.col-lg-8.mb-4.mb-md-0
              p El término “riesgo” se refiere a la posibilidad de desgaste o daño y sus posibles consecuencias. Estos riesgos pueden afectar a personas o grupos y son el resultado de un suceso o acción. Los riesgos se presentan tanto en ámbitos domésticos como laborales y sociales, entre otros.
              p La evaluación del riesgo implica considerar la vulnerabilidad frente a cada tipo de peligro. Es importante distinguir adecuadamente entre peligrosidad, vulnerabilidad y riesgo para gestionar adecuadamente cada situación.
  
      separador
      #t_4_1.titulo-segundo.mb-5
        h2 4.1 Seguridad y salud en el trabajo
  
      p La seguridad y salud en el trabajo se refiere a la prevención de lesiones y enfermedades causadas por las condiciones laborales, así como a la protección y promoción de la salud de los trabajadores. Para los cajeros en el punto de pago, es crucial implementar medidas específicas para garantizar su bienestar y seguridad, por ejemplo, adecuación de sistemas de vigilancia, prácticas seguras del manejo de efectivo, ergonomía, pausas activas, y un área de trabajo saludable.
      p Garantizar un ambiente seguro para el cajero en el puesto de pago y óptimas condiciones para el cuidado de su salud, son factores que propician su productividad y satisfacción laboral.
      p.mb-4 Consulte el video que se presenta a continuación, relacionado con las generalidades de la seguridad y salud en el trabajo, y el proceso integral que unifica las funciones de esta área en un sistema de gestión:
  
      .row.justify-content-center.align-items-center.mb-3
        .col-sm-12.col-md-12.col-lg-10
          figure
            .video
              iframe(iframe width="560" height="315" src="https://www.youtube.com/embed/RRSIdOpBJs4?si=x4TZRdBlI2KsWLoA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen)
            figcaption Video. Sistema de Gestión de la Seguridad y Salud en el Trabajo
  
      separador
      #t_4_2.titulo-segundo.mb-5
        h2 4.2 Protección de datos personales
  
      .row.justify-content-center.align-items-center.mb-2
        .col-6.col-md-2.col-lg-2
          .row.justify-content-center.align-items-center
            .col-12.col-md-11.col-lg-8
              img.mt-2.mb-2(src="@/assets/curso/temas/tema4/imagen1.png" alt="")
        .col-sm-12.col-md-12.col-lg-10
          p En Colombia, la protección de los datos personales se encuentra regulada principalmente por la Ley 1581 de 2012 y el Decreto 1074 de 2015. Estas normas establecen los principios, derechos y obligaciones relacionados con la recolección, el almacenamiento, el uso y la circulación de la información personal. 
          p Los datos personales corresponden a la información que identifica a una persona o que puede asociarse con ella. En el puesto de pago, esta información puede solicitarse para elaborar una factura, registrar al cliente en un programa de fidelización, aplicar un beneficio o gestionar una transacción.
  
  
    .container.tarjeta.tarjeta--blanca.bg02.p-4.p-md-5.borde-recto-abajo.borde-recto-arriba
  
      .row.justify-content-center.align-items-center
  
        .col-sm-12.col-md-12.col-lg-6
          p Los datos personales son toda la información asociada una persona y que permite su identificación:
          
          .row.align-items-center.justify-content-center
  
            .col-xl-4.col-lg-7.col-md-7.col-11.mb-4.mb-xl-0
              .crd_hover_txt(data-aos="flip-left").borde-redondo.bgblanco
                .row.align-items-center.justify-content-center
                  .col-4.col-md-3.col-lg-5
                    img.mt-3(src="@/assets/curso/temas/tema4/icon1-1.png", alt="")
                .row.align-items-center.justify-content-center
                  .col-10
                    p.mt-2.mb-3.text-center #[b Documento de identidad.]
  
            .col-xl-4.col-lg-7.col-md-7.col-11.mb-4.mb-xl-0
              .crd_hover_txt(data-aos="flip-left").borde-redondo.bgblanco
                .row.align-items-center.justify-content-center
                  .col-4.col-md-3.col-lg-5
                    img.mt-3(src="@/assets/curso/temas/tema4/icon1-2.png", alt="")
                .row.align-items-center.justify-content-center
                  .col-10
                    p.mt-3.mb-3.text-center #[b Datos de contacto.]
  
            .col-xl-4.col-lg-7.col-md-7.col-11.mb-4.mb-xl-0
              .crd_hover_txt(data-aos="flip-left").borde-redondo.bgblanco
                .row.align-items-center.justify-content-center
                  .col-4.col-md-3.col-lg-5
                    img.mt-2(src="@/assets/curso/temas/tema4/icon1-3.png", alt="")
                .row.align-items-center.justify-content-center
                  .col-10
                    p.mt-2.mb-3.text-center #[b Datos de facturación.]
  
          .row.align-items-center.justify-content-center.mt-3
  
            .col-xl-4.col-lg-7.col-md-7.col-11.mb-4.mb-xl-0
              .crd_hover_txt(data-aos="flip-left").borde-redondo.bgblanco
                .row.align-items-center.justify-content-center
                  .col-4.col-md-3.col-lg-5
                    img.mt-3(src="@/assets/curso/temas/tema4/icon1-4.png", alt="")
                .row.align-items-center.justify-content-center
                  .col-10
                    p.mt-3.mb-4.text-center #[b Información de fidelización.]
  
            .col-xl-4.col-lg-7.col-md-7.col-11.mb-4.mb-xl-0
              .crd_hover_txt(data-aos="flip-left").borde-redondo.bgblanco
                .row.align-items-center.justify-content-center
                  .col-4.col-md-3.col-lg-5
                    img.mt-3(src="@/assets/curso/temas/tema4/icon1-6.png", alt="")
                .row.align-items-center.justify-content-center
                  .col-10
                    p.mt-3.mb-4.text-center #[b Historial de compras.]
  
            .col-xl-4.col-lg-7.col-md-7.col-11.mb-4.mb-xl-0
              .crd_hover_txt(data-aos="flip-left").borde-redondo.bgblanco
                .row.align-items-center.justify-content-center
                  .col-4.col-md-3.col-lg-5
                    img.mt-3(src="@/assets/curso/temas/tema4/icon1-5.png", alt="")
                .row.align-items-center.justify-content-center
                  .col-12
                    p.mt-2.mb-3.text-center #[b Información de la transacción.]
  
        .col-11.col-md-10.col-lg-6
          img(src="@/assets/curso/temas/tema4/imagen2.png" alt="")
  
      p.mt-4 Existen datos sensibles que pueden afectar la intimidad de una persona o generar discriminación, como los relacionados con la salud, el origen racial o étnico, la orientación política, las convicciones religiosas, la afiliación sindical, la vida sexual y los datos biométricos. 
      p Su tratamiento está restringido y, salvo las excepciones establecidas por la ley, requiere autorización explícita del titular. Estos datos no deben solicitarse en el puesto de pago cuando no sean necesarios para la finalidad informada al cliente. 
  
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5.borde-recto-arriba
      .row.justify-content-center.align-items-center.mb-5
        .col-lg-4.mb-3.col-8
          img(src="@/assets/curso/temas/tema4/img01.png" alt="")
        .col-lg-8
          h5 Manejo de datos en el puesto de pago
          p Antes de solicitar información personal, se debe informar al cliente la finalidad para la cual será utilizada y solicitar su autorización cuando corresponda.
          p Durante la atención, el cajero debe:
          ul.lista-ul--color
            li.d-flex
              i.fas.fa-check-circle
              p.mb-0 Solicitar únicamente los datos necesarios.

            li.d-flex
              i.fas.fa-check-circle
              p.mb-0 Utilizar la información para la finalidad informada.

            li.d-flex
              i.fas.fa-check-circle
              p.mb-0 Evitar repetir en voz alta o exponer datos personales.

            li.d-flex
              i.fas.fa-check-circle
              p.mb-0 Proteger la confidencialidad de la información.

            li.d-flex
              i.fas.fa-check-circle
              p.mb-0 Utilizar solamente los sistemas autorizados por la organización.

            li.d-flex
              i.fas.fa-check-circle
              p.mb-0 Reportar cualquier pérdida, divulgación o uso inadecuado de los datos.

          .cajon.color-acento-contenido.p-4.mb-4
            p Los titulares tienen derecho a conocer, actualizar y rectificar su información, solicitar prueba de la autorización otorgada, conocer el uso dado a sus datos y solicitar su supresión o revocar la autorización cuando sea procedente. 
  
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
