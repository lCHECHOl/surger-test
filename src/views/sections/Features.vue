<template>
  <base-section
    id="features"
    class="secondary"
  >
    <v-responsive
      class="mx-auto"
      max-width="1350"
    >
      <v-container fluid>
        <v-row>
          <v-col
            v-for="card in cards"
            :key="card.title"
            cols="12"
            sm="4"
            md="4"
          >
            <base-info-card
              align="center"
              dark
              v-bind="card"
            />
          </v-col>
        </v-row>
      </v-container>
    </v-responsive>
  </base-section>
</template>

<script>
  export default {
    name: 'SectionFeatures',

    data: () => ({
      cards: [
        {
          icon: 'mdi-rocket-launch-outline',
          title: 'Misión',
          text: 'Aportar valor comercial, social y financiero tanto a clientes corporativos, internos y usuarios finales gracias a nuestro compromiso y expertise en el sector del Contact Center y BPO; siendo un puente óptimo que enlaza interacciones de calidad y personalizadas entre usuarios y colaboradores internos, de distintas edades, llenos de pasión y que han visto en el mundo del contact center una oportunidad de trascender las fronteras culturales y ampliar la forma de entender la era de las comunicaciones.',
        },
        {
          icon: 'mdi-eye-check-outline',
          title: 'Visión',
          text: 'Incorporar  diferentes tipos de operaciones de Contact Center a nuestra organización Inbound, OutBound, Redes Sociales y Cross Selling ampliando nuestra cartera de clientes corporativos en sectores como Telcos, Banca, E-Commerce y Salud. Así en el 2025 estaremos generando 450 puestos de trabajo en la zona Cafetera de Colombia Caldas, Antioquia y Quindío principalmente en pueblos donde podremos contribuir en proyectos de responsabilidad social y generación de empleos dignos y de calidad.',
        },
        {
          icon: 'mdi-bullseye-arrow',
          title: 'Objetivos',
          text: 'Incursionar en operaciones Inbound, Crosselling y Redes Sociales Incluir en nuestro portafolio de clientes Telecomunicaciones, Salud, Banca y Seguros y E-Commerce Crecimiento interno en factura y volumen de interacciones con clientes, generando un crecimiento semestral de 50% en nuevas plazas de trabajo. Ser pioneros en tema de responsabilidad social respecto a implementación de Contact Center en principales pueblos en Colombia. Ser expertos en entregar soluciones integrales en cada servicio',
        },
      ],
    }),
  }
</script>
