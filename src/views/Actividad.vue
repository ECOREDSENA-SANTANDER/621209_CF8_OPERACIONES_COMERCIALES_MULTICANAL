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
          mensaje_correcto: 'Ha acertado la respuesta.',
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
          mensaje_correcto: 'Ha acertado la respuesta.',
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
          mensaje_correcto: 'Ha acertado la respuesta.',
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
          mensaje_correcto: 'Ha acertado la respuesta.',
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
          mensaje_correcto: 'Ha acertado la respuesta.',
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
          mensaje_correcto: 'Ha acertado la respuesta.',
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
          mensaje_correcto: 'Ha acertado la respuesta.',
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
          mensaje_correcto: 'Ha acertado la respuesta.',
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
          mensaje_correcto: 'Ha acertado la respuesta.',
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
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 11,
          texto: 'El sistema neumático o <i>shut</i> se usa para:',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Leer el código de barras de los productos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Pesar mercancías en el puesto de pago.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Transportar cápsulas con dinero desde el puesto de pago hacia caja general o tesorería.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Registrar la clave personal del cliente.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 12,
          texto: 'El sistema transaccional en <i>retail</i> se entiende como:',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Un mueble destinado a exhibir productos cerca de la caja.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Un listado manual de precios sin relación con ventas.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Una norma exclusiva de seguridad ambiental.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Un conjunto de personas, procedimientos, <i>software</i>, bases de datos y dispositivos para registrar transacciones comerciales.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 13,
          texto:
            'Un puesto de trabajo adecuado para el cajero debe considerar:',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Ergonomía, comunicación, cajonera, efectivo suficiente, visibilidad y <i>stock</i> de útiles.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Ausencia de silla para evitar pausas durante la jornada.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Uso permanente de celulares personales en caja.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Ventanillas que impidan la comunicación con el cliente.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 14,
          texto: 'El manejo de valores en el <i>retail</i> se relaciona con:',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'La exhibición visual de productos en góndolas.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Las operaciones, registros y administración de efectivo y otros medios de pago.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'La decoración de vitrinas exteriores.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'La selección de proveedores de mercancía.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 15,
          texto: 'Los medios de pago son importantes porque:',
          imagen: require('@/assets/actividad/imagen05.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Eliminan la necesidad de entregar comprobantes.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Impiden que el cliente elija cómo cancelar su compra.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Permiten cancelar bienes, servicios o deudas de forma física o electrónica.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Solo funcionan cuando se paga en efectivo.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 16,
          texto:
            'La diferencia principal entre tarjeta débito y crédito es que:',
          imagen: require('@/assets/actividad/imagen6.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Ambas funcionan únicamente con dinero físico.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'La tarjeta débito financia compras y la tarjeta crédito descuenta de inmediato.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Ninguna requiere autorización de la entidad financiera.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'La tarjeta crédito financia compras; la tarjeta débito descuenta de la cuenta disponible.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 17,
          texto: 'Los códigos de pago permiten:',
          imagen: require('@/assets/actividad/imagen7.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Autorizar pagos electrónicos de facturas de forma rápida y segura.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Eliminar la identificación del cliente comprador.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Registrar productos sin precio en el inventario.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Desactivar alarmas de seguridad en las salidas.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 18,
          texto: 'La seguridad y salud en el trabajo para cajeros busca:',
          imagen: require('@/assets/actividad/imagen8.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Aumentar los tiempos de espera del cliente.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Prevenir riesgos laborales mediante condiciones seguras y saludables.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Omitir pausas activas durante la jornada.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Evitar el uso de prácticas seguras en el manejo de efectivo.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 19,
          texto:
            'En protección de datos, antes de usar información personal del cliente se debe:',
          imagen: require('@/assets/actividad/imagen9.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Compartirla libremente con terceros.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Solicitar datos sensibles sin explicación.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Solicitar autorización y manejar la información de forma transparente y segura.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Publicarla para fines comerciales sin consentimiento.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 20,
          texto: 'Un ejemplo de dato personal es:',
          imagen: require('@/assets/actividad/imagen10.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'El color del uniforme del cajero.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'La ubicación de la caja registradora.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'El tipo de papel de impresión.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'El documento de identidad, lugar de residencia o trayectoria académica de una persona.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
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
