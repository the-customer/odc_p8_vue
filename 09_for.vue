<script setup>



</script>

<template>
  <section class="card">
    <h2>13 - Lists</h2>

    <ul>
      <li v-for="p in products" :key="p.id">
        nomProduit - prixProduit FCFA
        <button>❌</button>
      </li>
    </ul>
  </section>
</template>

<style scoped>
.card { padding:16px; border:1px solid #eee; border-radius:12px; }
li { display:flex; justify-content:space-between; width:250px; }
button { border:none; background:none; cursor:pointer; }
</style>