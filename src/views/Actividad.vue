<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
      // Para cuestionario usar: ActividadController(:cuestionario="cuestionario") 
      // Para parrafo usar: ActividadController(:parrafo="parrafo")
      ActividadController(:cuestionario="cuestionario")
  </template>

<script>
import ActividadController from '@ecored-sena/base-kit/plugin/components/actividad/ActividadController.vue'

export default {
  name: 'ActividadDidactica',
  components: {
    ActividadController,
  },
  data: () => ({
    cuestionario: {
      tema: 'Recursos del cajero',
      titulo: 'Cuestionario',
      introduccion:
        '<b> Objetivo:</b> verificar la comprensión de los conceptos fundamentales relacionados con el rol del cajero, la organización del puesto de pago, la administración de dinero y documentos, el uso de equipos tecnológicos, los medios de pago, el manejo de valores, la seguridad y salud en el trabajo y la protección de datos personales en el <i>retail</i>. ',
      barajarPreguntas: true,
      titulo_aprobado: '¡BUEN TRABAJO!',
      titulo_reprobado: 'VUELVA A INTENTARLO',
      preguntas: [
        {
          id: 1,
          texto:
            'En el <i>retail</i>, el cajero cumple un papel representativo porque:',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Es el primer y último punto de contacto del cliente durante el proceso de compra.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Solo se encarga de almacenar mercancía en bodega.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Define los precios de todos los productos del establecimiento.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Reemplaza los protocolos de atención de la organización.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 2,
          texto: 'Una función esencial del cajero en el punto de pago es:',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Diseñar campañas publicitarias para el almacén.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Recibir, custodiar y registrar dinero, cheques u otros documentos de valor.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Modificar la política comercial sin autorización.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Decidir la compra de inventario para todas las áreas.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 3,
          texto:
            'Al organizar el puesto de pago antes de iniciar la atención, se debe:',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Mantener mercancía acumulada cerca de la caja.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Evitar revisar el funcionamiento del <i>software</i>.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Verificar conexión, papel, cajón, base entregada y acceso al sistema.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Dejar abierta la gaveta para agilizar la jornada.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 4,
          texto:
            'Después de finalizar una transacción en efectivo, una práctica segura consiste en:',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Guardar los comprobantes sin clasificarlos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Permitir que el cliente manipule la gaveta.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Omitir la entrega del cambio cuando hay fila.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Mantener cerrada la caja registradora para evitar hurtos.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 5,
          texto: 'La ética del cajero exige principalmente:',
          imagen: require('@/assets/actividad/imagen05.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Actuar con integridad, honradez, responsabilidad y confidencialidad.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto:
                'Utilizar información del punto de pago para beneficio personal.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Compartir datos de clientes sin autorización.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Aceptar procedimientos diferentes a los definidos por la empresa.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 6,
          texto: 'La terminal POS se utiliza en el puesto de pago para:',
          imagen: require('@/assets/actividad/imagen6.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Almacenar productos perecederos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Registrar productos, brindar información y recopilar datos de ventas.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Reemplazar las normas de protección de datos.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Transportar dinero hasta la tesorería.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 7,
          texto: 'Dentro de una terminal POS, la gaveta tiene como función:',
          imagen: require('@/assets/actividad/imagen7.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Imprimir el tiquete de compra.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Proporcionar información visual al cliente.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Guardar dinero, cheques y otros documentos de valor.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Pesar frutas y verduras en el punto de pago.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 8,
          texto: 'El <i>scanner</i> balanza aporta eficiencia porque:',
          imagen: require('@/assets/actividad/imagen8.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Solo permite consultar precios sin registrar ventas.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Sustituye todos los medios de pago.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Elimina la necesidad de atención al cliente.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Integra lectura de códigos y pesaje para registrar productos con rapidez y exactitud.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 9,
          texto: 'El datáfono se emplea principalmente para:',
          imagen: require('@/assets/actividad/imagen9.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Procesar pagos con tarjetas y comunicarse con entidades financieras para autorizar transacciones.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Desactivar dispositivos de seguridad de los productos.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Transportar dinero mediante cápsulas neumáticas.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Organizar billetes por denominación.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 10,
          texto:
            'El desactivador de <i>tags</i> evita molestias al cliente porque:',
          imagen: require('@/assets/actividad/imagen10.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Calcula automáticamente el cambio en efectivo.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Retira o desactiva dispositivos de seguridad después del registro de la compra.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Genera reportes de ventas al finalizar la jornada.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Sustituye la factura de venta.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 11,
          texto: 'El dispositivo <i>shut</i> cumple la función de:',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Clasificar automáticamente los billetes por denominación.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Imprimir comprobantes de pago.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Transportar de forma segura el dinero desde la caja hasta la tesorería.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Registrar códigos de barras de los productos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 12,
          texto:
            'En un establecimiento de <i>retail</i>, el <i>software</i> de caja permite principalmente:',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Controlar únicamente la iluminación del punto de venta.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Administrar exclusivamente la apertura de puertas automáticas.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Reemplazar totalmente la atención del cajero.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Registrar ventas, controlar inventarios y administrar las operaciones del punto de pago.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 13,
          texto: 'El arqueo de caja tiene como propósito principal:',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Verificar que el dinero existente coincida con los registros y detectar diferencias de <i>stock</i> de efectivo.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Eliminar la necesidad de registrar ventas.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Reemplazar los comprobantes de pago.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Modificar automáticamente los precios de los productos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 14,
          texto:
            'En el <i>retail</i>, una adecuada atención al cliente permite:',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Reducir la comunicación entre el cliente y la empresa.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Fortalecer la satisfacción, fidelización y confianza del consumidor.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Eliminar la necesidad de procesos de servicio.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Reemplazar el proceso de facturación.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 15,
          texto:
            'La comunicación asertiva durante el servicio al cliente favorece principalmente:',
          imagen: require('@/assets/actividad/imagen05.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'La generación de conflictos con los clientes.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'La disminución de la confianza en el establecimiento.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'La comprensión de las necesidades del cliente y una mejor experiencia de compra.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'La eliminación de protocolos de atención.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 16,
          texto:
            'Cuando se presenta una reclamación de un cliente, el cajero debe:',
          imagen: require('@/assets/actividad/imagen6.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Ignorar la situación para evitar demoras.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Responder con discusiones para defender el procedimiento.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Remitir siempre al cliente sin escucharlo.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Escuchar, mantener una actitud respetuosa y seguir el procedimiento establecido por la empresa.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 17,
          texto: 'El manejo adecuado del efectivo busca principalmente:',
          imagen: require('@/assets/actividad/imagen7.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Reducir riesgos de pérdida, fraude o errores en las transacciones.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Eliminar la necesidad de arqueos de caja.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Permitir que cualquier persona manipule la caja.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Reemplazar los controles internos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 18,
          texto:
            'La confidencialidad en el manejo de la información del cliente implica:',
          imagen: require('@/assets/actividad/imagen8.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Compartir libremente la información con otros clientes.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Proteger los datos personales y utilizarlos únicamente para los fines autorizados.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Publicar la información en redes sociales.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Eliminar todos los registros de compra.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 19,
          texto:
            'El cumplimiento de los protocolos de seguridad en caja permite:',
          imagen: require('@/assets/actividad/imagen9.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Incrementar los errores operativos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Eliminar el control del efectivo.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Proteger los recursos de la empresa y disminuir los riesgos durante la operación.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Evitar el registro de las ventas.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 20,
          texto: 'La calidad del servicio en caja se refleja cuando:',
          imagen: require('@/assets/actividad/imagen10.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Se atiende únicamente a los clientes frecuentes.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Se prioriza la rapidez sobre la exactitud de las transacciones.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Se omite la entrega de comprobantes para agilizar el proceso.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Se brinda una atención ágil, amable, segura y conforme a los procedimientos establecidos.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
      ],
      mensaje_final_aprobado: 'Ha superado la actividad. ',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica. ',
    },
  }),
}
</script>
