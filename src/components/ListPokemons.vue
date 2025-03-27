<script setup>
const pokemon = defineProps(["name", "urlBaseSvg"])
</script>

<template>
    <div class="col-4">
        <div class="card p-2 mb-3 cardListPokemon">
            <p class="text-center">{{ pokemon.name }}</p>
            <img 
            :src="urlBaseSvg" class="card-img-top" alt="..."
            height="80"/>
        </div>
    </div>
  
</template>

<style scoped>
.cardListPokemon{
    background: rgb(251,63,222);
background: radial-gradient(circle, rgba(251,63,222,0.7120973389355743) 0%, rgba(70,252,225,0.4740021008403361) 100%);
cursor: pointer;
}
.cardListPokemon:hover{
    background: rgb(251,63,222);
background: radial-gradient(circle, rgba(251,63,222,0.95) 0%, rgba(70,252,225,0.65) 100%);

}
.cardListPokemon img:hover{
    padding: .1rem;

}

</style>