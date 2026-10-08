<script setup>
import ProductCard from './ProductCard.vue'

const products = [
  { id: 1, name: 'Stylo', price: 500 },
  { id: 2, name: 'Cahier', price: 1500 },
  { id: 3, name: 'Classeur', price: 3500 },
]
</script>

<template>
  <section>
    <h2>15 - Props & Validators</h2>
    <p>Le parent envoie un objet <code>product</code> au composant enfant.</p>

    <div class="grid">
      <article class="card">
        <h3 class="name">{{ product[0].name }}</h3>
        <p class="price">{{ product[0].price.toLocaleString() }} FCFA</p>
        <p class="meta">ID: {{ product[0].id }}</p>
      </article>
    </div>
  </section>
</template>

<style scoped>
.grid { display: grid; gap: 12px; grid-template-columns: repeat(3, minmax(0, 1fr)); margin-top: 12px; }
@media (max-width: 900px) { .grid { grid-template-columns: 1fr; } }

.card { padding: 14px; border: 1px solid #eee; border-radius: 12px; background: #fff; }
.name { margin: 0; font-size: 16px; }
.price { margin: 6px 0 0; font-weight: 700; }
.meta { margin: 6px 0 0; color: #666; font-size: 12px; }
</style>