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
      tema: 'Microcontroladores y sensores',
      titulo: 'Cuestionario',
      introduccion:
        '<b> Objetivo:</b> Evaluar la comprensión y el uso adecuado de las herramientas básicas en la ventana <em>Board</em> del <em>software</em> EAGLE.',
      barajarPreguntas: true,
      titulo_aprobado: '¡BUEN TRABAJO!',
      titulo_reprobado: 'VUELVA A INTENTARLO.',
      preguntas: [
        {
          id: 1,
          texto:
            '¿Qué herramienta es fundamental en la atención al cliente para resolver dudas de manera inmediata?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'El correo postal.', esCorrecta: false },
            { id: 'b', texto: 'El teléfono.', esCorrecta: true },
            { id: 'c', texto: 'Las redes sociales.', esCorrecta: false },
            { id: 'd', texto: 'El fax.', esCorrecta: false },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 2,
          texto: '¿Cuál es un objetivo de la atención al cliente por teléfono?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Aumentar los tiempos de espera.',
              esCorrecta: false,
            },
            { id: 'b', texto: 'Ignorar las quejas.', esCorrecta: false },
            {
              id: 'c',
              texto: 'Proporcionar información clara y precisa.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Vender productos innecesarios.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 3,
          texto:
            '¿Qué actitud debe mantener un asesor durante una llamada telefónica?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Indiferencia.', esCorrecta: false },
            { id: 'b', texto: 'Agresividad.', esCorrecta: false },
            { id: 'c', texto: 'Empatía y respeto.', esCorrecta: true },
            { id: 'd', texto: 'Prisa por terminar.', esCorrecta: false },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 4,
          texto: '¿Qué es la escucha activa en el servicio al cliente?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Oír sin prestar atención.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Interrumpir constantemente al cliente.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Prestar atención total para comprender el mensaje.',
              esCorrecta: true,
            },
            { id: 'd', texto: 'Hablar más que el cliente.', esCorrecta: false },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 5,
          texto: '¿Cómo se debe saludar al iniciar una llamada profesional?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Diciendo solamente ""¿Aló?"".',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Con un saludo cordial, nombre de la empresa y nombre del asesor.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Preguntando directamente qué desea el cliente.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Sin saludar, esperando que el cliente hable.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 6,
          texto:
            '¿Qué se debe hacer si no se tiene la respuesta inmediata para un cliente?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Inventar una respuesta.', esCorrecta: false },
            { id: 'b', texto: 'Colgar la llamada.', esCorrecta: false },
            {
              id: 'c',
              texto:
                'Informar que se consultará y devolver la llamada lo antes posible.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Decirle al cliente que llame en otro momento.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 7,
          texto:
            '¿Cuál es un beneficio de la buena comunicación telefónica para la empresa?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Mejorar la imagen corporativa y fidelizar clientes.',
              esCorrecta: true,
            },
            { id: 'b', texto: 'Gastar más en telefonía.', esCorrecta: false },
            { id: 'c', texto: 'Tener menos llamadas.', esCorrecta: false },
            { id: 'd', texto: 'Aumentar las quejas.', esCorrecta: false },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 8,
          texto: '¿Qué se debe evitar al hablar por teléfono con un cliente?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Usar un lenguaje técnico excesivo o modismos.',
              esCorrecta: true,
            },
            { id: 'b', texto: 'Hablar con claridad.', esCorrecta: false },
            { id: 'c', texto: 'Ser amable.', esCorrecta: false },
            {
              id: 'd',
              texto: 'Llamar al cliente por su nombre.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 9,
          texto:
            '¿Qué elemento es vital para proyectar profesionalismo a través de la voz?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Gritar para que se escuche bien.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'El tono de voz y la modulación.',
              esCorrecta: true,
            },
            { id: 'c', texto: 'Hablar muy rápido.', esCorrecta: false },
            { id: 'd', texto: 'Usar un tono monótono.', esCorrecta: false },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 10,
          texto:
            '¿Cuál es el último paso recomendado al finalizar una llamada de servicio?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Colgar rápidamente.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Agradecer por la llamada y despedirse cordialmente.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Transferir a otra área sin avisar.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Preguntar por datos personales innecesarios.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 11,
          texto:
            '¿Qué herramienta permite registrar las interacciones con los clientes?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Un cuaderno personal.', esCorrecta: false },
            { id: 'b', texto: 'Un sistema CRM.', esCorrecta: true },
            { id: 'c', texto: 'La memoria del asesor.', esCorrecta: false },
            { id: 'd', texto: 'Una calculadora.', esCorrecta: false },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 12,
          texto: '¿Qué se debe hacer si el cliente está muy molesto?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Discutir con él.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Escuchar con calma y ofrecer soluciones.',
              esCorrecta: true,
            },
            { id: 'c', texto: 'Ignorar sus reclamos.', esCorrecta: false },
            { id: 'd', texto: 'Burlarse de su situación.', esCorrecta: false },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 13,
          texto: '¿Cómo influye la rapidez en la respuesta telefónica?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Genera insatisfacción.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Aumenta la percepción de eficiencia y calidad.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'No tiene ninguna importancia.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Hace que el cliente se asuste.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 14,
          texto: '¿Cuál es una característica de la comunicación asertiva?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Expresar ideas de forma clara y respetuosa.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Imponer el criterio propio a toda costa.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Quedarse callado ante las dudas.',
              esCorrecta: false,
            },
            { id: 'd', texto: 'Ser sarcástico.', esCorrecta: false },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 15,
          texto: '¿Por qué es importante el seguimiento tras la llamada?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Para asegurar que la solicitud del cliente se resolvió.',
              esCorrecta: true,
            },
            { id: 'b', texto: 'Para molestar al cliente.', esCorrecta: false },
            {
              id: 'c',
              texto: 'Para llenar espacio en la base de datos.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Para cobrar cargos adicionales.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
      ],
      mensaje_final_aprobado: '¡Excelente! Ha superado la actividad.',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
}
</script>
