<template>
  <div class="item-form-container">
    <div class="item-form-container-block">
      <div class="red-mark-div">
        <p class="input-description">
          Наименование товара
        </p>
        <div class="red-mark" />
      </div>
      <input class="item-form-container-block-input" type="text" placeholder="Введите наименование товара">
    </div>
    <div class="item-form-container-block">
      <p class="input-description">
        Описание товара
      </p>
      <textarea class="item-form-container-block-input item-form-container-block-input-big" placeholder="Введите описание товара" />
    </div>
    <div class="item-form-container-block">
      <div class="red-mark-div">
        <p class="input-description">
          Ссылка на изображение
        </p>
        <div class="red-mark" />
      </div>
      <input class="item-form-container-block-input" type="text" placeholder="Введите ссылку">
    </div>
    <div class="item-form-container-block">
      <div class="red-mark-div">
        <p class="input-description">
          Цена товара
        </p>
        <div class="red-mark" />
      </div>
      <input class="item-form-container-block-input" type="text" placeholder="Введите цену">
    </div>
    <div class="item-form-container-button">
      <p class="item-form-container-button-text">
        Добавить товар
      </p>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      itemName: ''
    }
  },
  methods: {
    onFocus () {
      if (this.itemName.onFocus) {
        this.itemName.border = 4
      }
    }
  }
}
</script>

<style>
.item-form-container {
  width: 284px;
  height: 392px;
  background-color: rgba(255, 254, 251, 1);
  box-shadow: 0px 6px 10px 0px rgba(0, 0, 0, 0.02), 0px 20px 30px 0px rgba(0, 0, 0, 0.04);
  border-radius: 4px;
  margin-top: 16px;
  padding: 24px;
  position: sticky;
  top: 24px;
}

.item-form-container .item-form-container-block:not(:first-child){
  margin-top: 16px;
}

.item-form-container-block {
  font-weight: 400;
  font-size: 10px;
  line-height: 12.5px;
  color: rgba(73, 72, 94, 1);
}

.input-description {
  margin: 0;
  margin-bottom: 4px;
}

.item-form-container-block-input {
  width: 100%;
  box-sizing: border-box;
  border-radius: 4px;
  border-style: none;
  box-shadow: 0px 2px 5px 0px rgba(0, 0, 0, 0.1);
  height: 36px;
  color:rgba(63, 63, 63, 1);
  padding: 0;
  font-family: 'Source Sans Pro', sans-serif;
  padding-left: 16px;
  font-weight: 400;
  font-size: 12px;
  line-height: 15px;
}

.item-form-container-block-input-big {
  height: 108px;
  resize: none;
  font-family: 'Source Sans Pro', sans-serif;
  padding-top: 10px;
  padding-right: 16px;
}

.item-form-container-block-input::placeholder {
  color: rgba(180, 180, 180, 1);
  font-family: 'Source Sans Pro', sans-serif;
  font-weight: 400;
  font-size: 12px;
  line-height: 15px;
  margin: 0;
}

.red-mark-div {
  display: flex;
  flex-flow: row;
}

.red-mark {
  height: 4px;
  width: 4px;
  border-radius: 2px;
  background-color: rgba(255, 132, 132, 1);
  margin-top: 0;
}

.item-form-container-button {
  display: flex;
  align-content: center;
  justify-content: center;
  height: 36px;
  width: 284px;
  border-radius: 10px;
  background-color: rgba(238, 238, 238, 1);
  margin-top: 24px;
}

.item-form-container-button-text {
  font-weight: 600;
  font-size: 12px;
  font-family: 'Inter', sans-serif;
  color: rgba(180, 180, 180, 1);
}
</style>
