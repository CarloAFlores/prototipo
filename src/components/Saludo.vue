<template>
  <section class="header">
    <div class="header__text"><p>Hola {data}, !Nos encanta que estes aqui!</p></div>
    <div class="header__text_bold">Restaurante:<p class="text__bold">{data}</p>/ Mesa:<p class="text__bold">{data}</p></div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.header{
  margin-top: 5%;
  display: flex;
  flex-direction: column;
  align-items: center;
  .header__text{
    font-weight: 900;
    color: var(--negro );
  }
  .header__text_bold{
    display: flex;
    margin-left: -6.5rem;
    color: var(--negro );
    font-size: 80%;
    .text__bold{
      font-weight: bolder;
    }
  }

}

</style>