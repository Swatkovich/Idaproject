<template>
  <div class="header">
    <h1 class="title">
      Добавление товара
    </h1>
    <div class="psevdoButton">
      <p class="psevdoButton-text">
        По умолчанию
      </p>
      <svg class="psevdoButton-arrow" viewBox="0 0 8 6" xmlns="http://www.w3.org/2000/svg">
        <path d="M7.48532 1.24264L4.24268 4.48528L1.00003 1.24264" stroke="#B4B4B4" />
      </svg>
    </div>
  </div>
</template>

<script>
</script>

<style>
.header {
  display: flex;
  flex-flow: row;
  justify-content: space-between;
  margin: 0;
}

.title {
  margin: 0;
  font-weight: 600;
  line-height: 35.2px;
  font-size: 28px;
  color: rgba(63, 63, 63, 1);
}

.psevdoButton {
  height: 36px;
  width: 122px;
  border-radius: 4px;
  background-color: rgba(255, 254, 251, 1);
  box-shadow: 0px 2px 5px 0px rgba(0, 0, 0, 0.1);
  display: flex;
  justify-content: center;
  /* align-items: center; */
}

.psevdoButton-text {
  font-weight: 400;
  font-size: 12px;
  line-height: 15px;
  color: rgba(180, 180, 180, 1);
  margin: 0px 5px 0px 0px;
  margin-top: 10px;
}

.psevdoButton-arrow {
  width: 8px;
  height: 6px;
  fill: none;
  margin-top: 16px;
}
</style>
