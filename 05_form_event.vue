<script setup>

</script>

<template>
  <div class="card">
    <h3>EventForm</h3>

    <form class="form" @submit.prevent="submit">
      <input class="input" placeholder="Nom complet" />
      <input class="input" placeholder="Téléphone" />
      <button type="submit">Enregistrer</button>
    </form>

    <p class="note">
      Démo : <code>...</code>, <code>...</code>.
    </p>
  </div>
</template>

<style scoped>
.card { padding: 14px; border: 1px solid #eee; border-radius: 12px; margin-top: 12px; }
.form { display: flex; gap: 10px; flex-wrap: wrap; }
.input { padding: 8px 10px; border: 1px solid #ddd; border-radius: 10px; min-width: 220px; }
button { padding: 8px 10px; border-radius: 10px; border: 1px solid #ddd; background: white; }
.empty { margin-top: 10px; color: #666; }
.list { margin: 10px 0 0; padding-left: 18px; }
.note { margin-top: 8px; color: #555; }
</style>