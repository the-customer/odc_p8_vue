<script setup>

</script>

<template>
  <section class="card">
    <h2>12 - Conditional Rendering</h2>

    <p>
      🛒 Panier vide
    </p>

    <ul>
      <li v-for="(i, index) in items" :key="index">
        {{ i }}
      </li>
    </ul>

    <button>
      Ajouter produit
    </button>
  </section>
</template>

<style scoped>
.card { padding:16px; border:1px solid #eee; border-radius:12px; }
button { margin-top:10px; padding:8px 10px; }
</style>