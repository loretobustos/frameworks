<template>
  <div>
    <b-container class="bv-example-row">
      <b-row>
        <b-col md="4" v-for="personaje in personajes" :key="personaje.nombre">
          <b-card


            :img-src="personaje.imagen"
            img-alt="Image"
            img-top
          >
            <b-card-text>
              {{ personaje.nombre }}
            </b-card-text>
          </b-card></b-col
        >
      </b-row>
    </b-container>

  </div>
</template>


<script>
export default {
  name: "component-name",
  // props: {},
  data: function () {
    return {
      personajes: [
        {
          id: 1,
          nombre: "Morty",
          imagen: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
        },
        {
          id: 2,
          nombre: "Rick",
          imagen: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
        },
        {
          id: 3,
          nombre: "Summer",
          imagen: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
        },
        {
          id: 4,
          nombre: "Beth",
          imagen: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
        },
        {
          id: 5,
          nombre: "Jerry",
          imagen: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
        },
      ],
    };
  },
  // computed: {},
  methods: {
    // -- Metodos
  },
  // components: {},
};
</script>

<style scoped>
</style>