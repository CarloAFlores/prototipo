<template>
  <section class="cabezera">
    <button @click="this.$router.go(-1)" class="regresar"> <img src="@/assets/arrow_back.svg" class="arrow_back"> </button>
    <img src="@/assets/adidas.png" class="logo">
    <div></div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.cabezera{
  background: rgb(56, 54, 54);
  display: flex;
  align-items: center;
  justify-content: space-between;
  position: sticky;
  top: 0;
  z-index: 1;
  
  .regresar{
    width: 6%;
    background: transparent;
    border: none;
    .arrow_back{
      width: 100%;
    }
  }
  .logo{
    width:15%;
    height:20%;
  }
}

</style>