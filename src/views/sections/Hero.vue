<template>
  <section id="hero">
    <v-img
      :min-height="minHeight"
      :src="require('@/assets/light.jpg')"
      class="white--text"
      gradient="to bottom, rgba(11, 28, 61, .9), rgba(0,0,0,.4)"
    >
      <v-container class="fill-height px-4 py-12">
        <v-responsive
          class="d-flex align-center mx-auto"
          height="100%"
          max-width="700"
          width="100%"
        >
          <base-subheading
            weight="regular"
            title="SOMOS EL GRAN ALIADO PARA EL CRECIMIENTO DE TU EMPRESA"
          />

          <base-heading
            size="text-h2"
            title="SURGER CONTACT CENTER"
            weight="medium"
          />

          <base-body>
            Aportamos valor comercial, social y financiero tanto a clientes corporativos, internos y usuarios finales gracias a nuestro compromiso y expertise en el sector del Contact Center y BPO
          </base-body>


        </v-responsive>
      </v-container>
    </v-img>
  </section>
</template>

<script>
  export default {
    name: 'SectionHero',

    provide: {
      theme: { isDark: true },
    },

    computed: {
      minHeight () {
        const height = this.$vuetify.breakpoint.mdAndUp ? '100vh' : '50vh'

        return `calc(${height} - ${this.$vuetify.application.top}px)`
      },
    },
  }
</script>
