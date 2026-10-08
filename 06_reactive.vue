<script setup>

</script>

<template>
  <section class="card">
    <h2>09 - reactive()</h2>

    <div class="box">
      <p><strong>Nom :</strong> ... </p>
      <p><strong>Téléphone :</strong> ... </p>
      <p><strong>Solde :</strong> ... FCFA</p>
    </div>

    <div class="actions">
      <button>+5 000</button>
      <button>+10 000</button>
    </div>

    <p class="note">
      <code>reactive()</code> est idéal pour les objets complexes.
    </p>
  </section>
</template>

<style scoped>
.card { padding:16px; border:1px solid #eee; border-radius:12px; }
.box { padding:12px; background:#fafafa; border-radius:10px; }
.actions { display:flex; gap:10px; margin-top:10px; }
button { padding:8px 10px; border:1px solid #ddd; border-radius:8px; }
.note { margin-top:8px; color:#555; }
</style>