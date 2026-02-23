<template lang="pug">
.curso-main-container.introduccion
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido(data-aos="flip-up")
      .titulo-principal__numero
        span
          i.fas.fa-info
      h1 Introducción

    //- Párrafo superior
    p.mb-4(data-aos="fade-up") En la sociedad actual, el teléfono es una herramienta fundamental empleada en diversas actividades tanto personales como empresariales. La comunicación telefónica se ha convertido en un recurso cotidiano dentro de cualquier organización, siendo uno de los elementos clave en un buen esquema de atención al cliente.

    //- Bloque central estilo Banner/Imagen con recuadro
    .bloque-texto-g.color-primario.p-3.p-sm-4.p-md-5.mb-5(data-aos="flip-down")
      .bloque-texto-g__img(
        :style="{'background-image': `url(${require('@/assets/curso/tema1/img2.png')})`}"
      )
      .bloque-texto-g__texto.p-4
        p.mb-0 Aunque comúnmente se piensa que comunicarse por teléfono es tarea fácil por tratarse de un hábito tradicional, lo cierto es que cuando esta se realiza de forma profesional, requiere habilidades específicas y preparación. Por esta razón, es fundamental formarse en este campo para lograr una comunicación efectiva y profesional.

    //- Párrafo inferior
    p.mb-5(data-aos="fade-up") En un mercado saturado de mensajes visuales y gráficos, el teléfono ofrece una vía directa para transmitir una buena imagen empresarial. Usado correctamente, puede traer importantes beneficios organizacionales como la consolidación de relaciones con clientes, gracias a su capacidad para ofrecer una comunicación rápida, continua y eficaz.
    
    //- SECCIÓN 1.1 (Todo esto debe llevar la misma indentación que los párrafos de arriba)
    .mt-5
      .titulo-segundo.color-acento-contenido(data-aos="fade-right")
        h2 1.1 El papel del asesor en la comunicación telefónica

      p.mb-4(data-aos="fade-up") El rol del asesor o asesora telefónica es esencial en la atención al cliente, ya que su única herramienta de trabajo es la voz. Esto implica que debe poseer, desarrollar o fortalecer ciertas cualidades que le permitan brindar una atención eficiente y profesional.

      //- Bloque de texto con imagen (Fondo Amarillo)
      .bloque-texto-g.color-acento-botones.p-3.p-sm-4.p-md-5.mb-5(data-aos="flip-down")
        .bloque-texto-g__img(
          :style="{'background-image': `url(${require('@/assets/curso/tema1/img3.png')})`}"
        )
        .bloque-texto-g__texto.p-4
          p.mb-0 Todas las personas pueden ser capacitadas para desempeñar tareas que exijan un perfil comercial y de servicio, siempre que tengan las cualidades necesarias o estén dispuestas a desarrollarlas con esfuerzo y dedicación. Aunque algunas de estas habilidades pueden estar presentes de manera natural, en muchos casos deben ser cultivadas.

      p.mb-4(data-aos="fade-up") A continuación, se presentan las cualidades necesarias para desempeñarse adecuadamente como asesor o asesora telefónica:

      //- Fila de tarjetas de cualidades
      .row.justify-content-center
        - 
          const cualidades = [
            'Ganas de aprender',
            'Interés por el trabajo',
            'Excelente trato con el cliente',
            'Gran sentido del respeto',
            'Empatía',
            'Paciencia'
          ]
        each item, index in cualidades
          .col-6.col-md-4.col-lg-2.mb-3(data-aos="fade-in" :data-aos-delay="index * 100")
            .tarjeta.tarjeta--azul-clara.p-3.h-100.d-flex.align-items-center.justify-content-center.text-center
              p.mb-0.fw-bold= item
      .mb-4(data-aos="fade-in") Estas cualidades son fundamentales para que el asesor o asesora pueda interpretar las necesidades del cliente, responder con claridad y mantener un trato respetuoso, incluso en situaciones complejas. Cada llamada representa una oportunidad para fortalecer la confianza y generar experiencias positivas con los clientes.
      .mb-4 
      .mb-4 El cliente es lo primero

    
      

</template>

<script>
export default {
  name: 'Tema1',
  data: () => ({
    mostrarIndicadorTarjetaAudio: true,
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
