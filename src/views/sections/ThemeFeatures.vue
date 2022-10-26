<template>
  <base-section id="theme-features">
    <base-section-heading title="Nuestros Servicios">
      Te presentamos nuestro portafolio de servicios
    </base-section-heading>

    <v-container>
      <v-row>
        <v-col
          v-for="(feature, i) in features"
          :key="i"
          cols="12"
          md="6"
        >
          <base-avatar-card
            v-bind="feature"
            align="left"
            horizontal
          >
            {{ feature.desc}}
          </base-avatar-card>
        </v-col>
      </v-row>
    </v-container>
  </base-section>
</template>

<script>
  export default {
    name: 'SectionThemeFeatures',

    data: () => ({
      features: [
        {
          title: 'Ventas',
          icon: 'mdi-finance',
          desc: 'Combinamos ventas tradicionales con canales más eficientes, aumentando su crecimiento como empresa',
        },
        {
          title: 'Gestion de cobranzas',
          icon: 'mdi-cash-check',
          desc: 'Tenemos como objetivo reactivar la relacion comercial con los clientes ofreciendo alternativas de negociación y solución para cada caso',
        },
        {
          title: 'Atención al cliente PQR',
          icon: 'mdi-email-alert-outline',
          desc: 'Ayudamos de manera eficiente a desarrollar una relacion con el cliente positiva con su compañia',
        },
        {
          title: 'Back Office',
          icon: 'mdi-laptop',
          desc: 'Trabajamos en que todos los angulos de las gestiones comerciales puedan tener una trazabilidad y fiabilidad de las operaciones',
        },
        {
          title: 'Redes Sociales',
          icon: 'mdi-account-supervisor',
          desc: '',
        },
        {
          title: 'Crosseling',
          icon: 'mdi-chart-multiple',
          desc: '',
        },
        {
          title: 'Soporte 24/7',
          icon: 'mdi-phone-clock',
          desc: 'Brindamos el servicio sin importar el lugar donde te encuentres o la zona horaria en la que estes',
        },
      ],
    }),
  }
</script>
