<template>
  <div class="container mt-5 text-body-secondary">
    <div class="card shadow-lg border-0">
      <div class="card-header bg-primary text-white text-center">
        <h1 class="fw-bold">🔍 Descubra o Mundo Pokémon com PokeVite!</h1>
      </div>
      <div class="card-body pb-4">
        <p class="lead">
          Bem-vindo ao <strong>PokeVite</strong>! Uma aplicação web interativa criada para os verdadeiros treinadores Pokémon.
          Aqui você pode pesquisar seus Pokémon favoritos, visualizar estatísticas detalhadas e explorar novas criaturas de forma dinâmica.
        </p>
        <hr />
        <h4 class="text-primary">🚀 Tecnologias Utilizadas</h4>
        <ul>
          <li><strong>Vue 3</strong> – Para uma experiência reativa e dinâmica.</li>
          <li><strong>Vite</strong> – Para um build ultrarrápido e eficiente.</li>
          <li><strong>Bootstrap</strong> – Para um design responsivo e elegante.</li>
          <li><strong>PokéAPI</strong> – Para obter todas as informações do universo Pokémon.</li>
        </ul>
        <hr />
        <h4 class="text-success">🎯 Objetivo do Projeto</h4>
        <p class="mb-4">
          O PokeVite foi desenvolvido para melhorar minhas habilidades em <strong>consumo de APIs REST</strong>, 
          otimização de aplicações frontend e criação de interfaces modernas e intuitivas.
        </p>
      </div>
    </div>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}

.card {
  border-radius: 12px;
}

.card-header {
  border-top-left-radius: 12px;
  border-top-right-radius: 12px;
}
</style>
