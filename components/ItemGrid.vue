<template>
  <div class="item-grid">
    <myItemCard
      v-for="(card, i) in $store.state.cards"
      :key="i"
      :card="card"
    />
    <ItemCard />
    <ItemCard />
    <ItemCard />
    <ItemCard />
    <ItemCard />
    <ItemCard />
    <ItemCard />
    <ItemCard />
  </div>
</template>

<script>
</script>

<style>
.item-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 16px;
  margin-top: 16px;
  margin-left: 16px;
}
</style>
