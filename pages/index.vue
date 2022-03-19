<template>
  <div class="container">
    <MyHeader />
    <div class="items-container">
      <ItemForm />
      <ItemGrid />
    </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>

<style>
body {
  display: flex;
  flex-flow: column;
  background-color: rgb(230, 230, 230);
  margin: 0;
  align-items: center;
}

.container {
  background-color: rgba(255, 254, 251, 0.8);
  margin: 0;
  width: 1376px;
  height: 100%;
  font-family: 'Source Sans Pro', sans-serif;
  padding: 32px;

}

.items-container {
  display: flex;
  flex-flow: row;
}

</style>
