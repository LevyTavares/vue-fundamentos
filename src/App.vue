<script setup>
  import ProductCard from './components/ProductCard.vue';
</script>

<template>
<main>
  <h1>Catálogo de Produtos</h1>

  <form>
    <div>
      <label for="nome">Nome</label>
      <input id="nome" type="text" required/>
    </div>
    <div>
      <label for="descricao">Descrição</label>
      <input id="descricao" type="text" required/>
    </div>
    
    <div>
      <label for="preco">Preço</label>
      <input id="preco" type="text" required/>
    </div>
    <div>
      <label for="imagem">Imagem URL</label>
      <input id="imagem" type="text" required/>
    </div>
    <div>
      <button type="submit">Adicionar Produto</button>
    </div>
  </form>

  <ProductCard/>
</main>
</template>

<style scoped>
  form {
    margin-top: 1rem;
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
  }
  form label{
    display: block;
    margin-bottom: .2rem;
  }
  form input {
    box-sizing: border-box;
    padding: .5rem;
    width: 100%;
  }
  button {
    padding: .5rem;
    background-color: #007BFF;
    color: white;
    border: none;
    border-radius: 5px;
    max-width: 200px;
    margin-left: auto;
    cursor: pointer;
  }
</style>
