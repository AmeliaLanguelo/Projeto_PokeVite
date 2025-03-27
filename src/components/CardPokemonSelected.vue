<script setup>
const pokemon = defineProps(["name", "xp", "height", "img", "loading"])
</script>

<template>
          <div class="card CardPokemonSelected" 
          :class="loading? '' : 'animate__animated animate__flipInX'"
          >
            
            <img 
            v-if="pokemon.name"
            :src="pokemon.img" 
            height="250"
            class="card-img-top pt-12" 
            :alt="pokemon.name">

            <img 
            v-else
            src="../assets/egg_pokemon.svg" 
            height="250"
            class="card-img-top pt-12" 
            alt="???">

            <div class="card-body">
              <h5 class="card-title text-center">{{ pokemon.name || '???' }}</h5>
              <hr>
              <div class="row">
                <section class="col">
                    <strong>XP:</strong>
                    <span>{{ pokemon.xp }}</span>
                </section>
                <section class="col">
                    <strong>Altura:</strong>
                    <span>{{ pokemon.height }}</span>
                </section>
              </div>
              
            </div>
          </div>

</template>

<style scoped>
.CardPokemonSelected{
  height: 74vh;
  background: rgb(251,63,222);
  background: radial-gradient(circle, rgba(222, 199, 108, 0.9) 0%, rgba(233, 111, 111, 0.4) 100%);
}

</style>