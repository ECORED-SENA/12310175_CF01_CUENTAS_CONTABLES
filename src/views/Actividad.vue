<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
  
      #Actividad                
        <Actividad :cuestionario="cuestionario"/>
  
  </template>

<script>
import Actividad from 'ecored-pkg-fliz/plugin/components/actividad/Actividad.vue'
export default {
  name: 'ActividadDidactica',
  components: {
    Actividad,
  },
  data: () => ({
    cuestionario: {
      tema: 'Cuentas contabless',
      titulo: 'Cuestionario',
      introduccion:
        '<b> Objetivo:</b> Identificar los conceptos esenciales sobre las cuentas contables, registros contables, estados de ingresos y egresos y algunos aspectos fundamentales.',
      barajarPreguntas: true,
      titulo_aprobado: '¡BUEN TRABAJO!',
      titulo_reprobado: 'VUELVA A INTENTARLO.',
      preguntas: [
        {
          id: 13,
          texto: '¿Cuál de los siguientes elementos pertenece al activo?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Cuentas por pagar.', esCorrecta: false },
            { id: 'b', texto: 'Capital social.', esCorrecta: false },
            { id: 'c', texto: 'Caja.', esCorrecta: true },
            { id: 'd', texto: 'Préstamos bancarios.', esCorrecta: false },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 14,
          texto:
            '¿Cuál de las siguientes situaciones representa un pasivo para la empresa?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Un préstamo pendiente con una entidad financiera.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Dinero en banco disponible para retiro de la empresa.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Mercancía para la venta directa o entregar en consignación.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Equipos de oficina para la operación de la empresa.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 15,
          texto: 'El patrimonio de una empresa aumenta cuando:',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Se adquiere una deuda.', esCorrecta: false },
            { id: 'b', texto: 'Se generan utilidades.', esCorrecta: true },
            { id: 'c', texto: 'Se pagan obligaciones.', esCorrecta: false },
            { id: 'd', texto: 'Se disminuyen los activos.', esCorrecta: false },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 16,
          texto: '¿Cuál de los siguientes es un ejemplo de pasivo?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Inventarios.', esCorrecta: false },
            { id: 'b', texto: 'Clientes.', esCorrecta: false },
            { id: 'c', texto: 'Proveedores.', esCorrecta: true },
            { id: 'd', texto: 'Equipos.', esCorrecta: false },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 17,
          texto:
            'Si una empresa tiene activos por $100.000 y pasivos por $40.000, su patrimonio es:',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: '$140.000.', esCorrecta: false },
            { id: 'b', texto: '$40.000.', esCorrecta: false },
            { id: 'c', texto: '$100.000.', esCorrecta: false },
            { id: 'd', texto: '$60.000.', esCorrecta: true },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 18,
          texto: 'Cuando una empresa paga una deuda, ¿qué ocurre?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Disminuye el activo y el pasivo.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Aumenta el activo y el pasivo.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Aumenta el patrimonio y el gasto.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'No hay ningún cambio, sin novedades.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 19,
          texto: 'Las cuentas del activo se caracterizan por:',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Aumentar en el haber y disminuir en el debe.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Aumentar en el debe y disminuir en el haber.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Aumentar y disminuir únicamente en el debe.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'No tener ningún movimiento contable.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 20,
          texto:
            'Las cuentas de pasivo y patrimonio presentan el siguiente comportamiento:',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Aumentan en el debe y disminuyen en el haber.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Solo aumentan en el debe, por su naturaleza.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'No disminuyen nunca, permanecen estáticas.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Aumentan en el haber y disminuyen en el debe.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
      ],
      mensaje_final_aprobado: '¡Excelente! Ha superado la actividad.',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
}
</script>
