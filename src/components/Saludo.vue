<template>
  <section class="saludo">
    <div class="name"><p>Hola {data}, !Nos encanta que estes aqui!</p></div>
    <div class="datos">Restaurante: <p class="dato">{data}</p>/ Mesa <p class="dato">{data}</p></div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss">
.saludo{
  display: flex;
  flex-direction: column;
  align-items: center;
  font-size: 1.3rem;
  margin-top: 6%;
  font-family: AvenirLTStd-book;
  .name{
    text-align: center;
  }
  .datos{
    display: flex;
    font-size: 1rem;
    .dato{
      font-weight: bold;
    }
  }
}
</style>