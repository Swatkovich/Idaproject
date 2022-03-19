<template>
  <div class="item-card">
    <img class="item-card-image" src="/item_image.png" alt="Item Picture.png">
    <div class="item-card-information">
      <p class="item-card-name">
        Наименование товара
      </p>
      <p class="item-card-description">
        Довольно-таки интересное описание товара в несколько строк. Довольно-таки интересное описание товара в несколько строк
      </p>
      <p class="item-card-price">
        10 000 руб.
      </p>
      <div class="item-card-delete_button">
        <img class="item-card-delete_button-svg" src="/delete_icon.svg" alt="X">
      </div>
    </div>
  </div>
</template>

<script>

</script>

<style>
.item-card {
  display: flex;
  flex-flow: column;
  width: 332px;
  height: 423px;
  border-radius: 4px;
  background-color: rgba(255, 254, 251, 1);
  box-shadow: 0px 6px 10px 0px rgba(0, 0, 0, 0.02), 0px 20px 30px 0px rgba(0, 0, 0, 0.04);
}

.item-card-image {
  height: 200px;
  border-top-right-radius: 4px;
  border-top-left-radius: 4px;
}

.item-card-information {
  display: flex;
  flex-flow: column;
  padding: 16px 16px 24px 16px;
}

.item-card-name {
  font-size: 20px;
  line-height: 25px;
  font-weight: 600;
  margin: 0;
}

.item-card-description {
  font-size: 16px;
  line-height: 20px;
  font-weight: 400;
  margin: 0;
  margin-top: 16px;
}

.item-card-price {
  font-size: 24px;
  line-height: 30px;
  font-weight: 600;
  margin: 0;
  margin-top: 32px;
}

.item-card-delete_button {
  display: none;
  height: 32px;
  width: 32px;
  position: relative;
  top: -407px;
  left: 292px;
  border-radius: 10px;
  background-color: rgba(255, 132, 132, 1);
  margin: 0;
  cursor: pointer;
}

.item-card-delete_button-svg {
  font-size: 20px;
  position: relative;
  left: 8px;
  top: 8px;
}

.item-card:hover .item-card-delete_button{
  display: block;
}

</style>
