<template>
<section class="container">

  <button><img src="@/assets/arrow_return.svg" ></button>
  <img src="@/assets/adidas.png" class="container__img">
  <div></div>

</section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.container{
  background: rgb(146, 137, 137);
  display: flex;
  justify-content: space-between;
  align-items: center;
  .container__img{
    width: 20%;
  }
}
</style>