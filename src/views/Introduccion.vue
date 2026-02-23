<template lang="pug">
.curso-main-container.introduccion
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido(data-aos="flip-up")
      .titulo-principal__numero
        span
          i.fas.fa-info
      h1 Introducción

    .row.justify-content-center.align-items-center.mb-5
      .col-12(data-aos="fade-right")
        p La comunicación telefónica ocupa un lugar central en las dinámicas actuales de atención al cliente, tanto en el ámbito personal como en el organizacional. A través del teléfono se construyen percepciones, se transmiten mensajes clave y se consolida la imagen de una empresa frente a sus clientes y usuarios. Por esta razón, su uso requiere preparación, actitud profesional y dominio de habilidades comunicativas específicas.

    .row.justify-content-center.align-items-stretch
      //- Bloque izquierdo con fondo verde claro
      .col-lg-4.mb-4.mb-lg-0(data-aos="fade-right")
        .p-4.h-100(style="background-color: #D2F3E8; border-radius: 15px;")
          p.mb-0 Aunque suele asumirse como una práctica cotidiana, la comunicación telefónica demanda un manejo consciente de la voz, el lenguaje y la escucha activa. El asesor o la asesora debe interpretar necesidades, responder con claridad y mantener un trato respetuoso, incluso en situaciones complejas. Cada llamada representa una oportunidad para fortalecer la confianza y generar experiencias positivas.

      //- Bloque central con la imagen
      .col-lg-4.mb-4.mb-lg-0(data-aos="zoom-in")
        figure
          img(src='@/assets/curso/intro/img1.png', alt='Asesora de servicio al cliente con audífonos')

      //- Bloque derecho con icono y texto
      .col-lg-4(data-aos="fade-left")
        .row.mb-3
          .col-auto
            figure
              img(src='@/assets/curso/intro/icono1.svg', alt='Icono comunicación', style="width: 70px;")
        p Formarse en comunicación telefónica permite desarrollar competencias orientadas al servicio, la empatía y la organización del diálogo. El adecuado manejo de las etapas de la llamada, los tipos de clientes y las técnicas básicas contribuye a una atención coherente con los objetivos institucionales y con las expectativas del cliente, favoreciendo relaciones sostenibles y profesionales.

</template>

<script>
export default {
  name: 'Introduccion',
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
