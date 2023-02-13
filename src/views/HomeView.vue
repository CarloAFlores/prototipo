<template>
  <HelloWorld/>
  <Saludo/>

  <div class="pregunta"><p>Cuantas persona se encuentra en tu mesa?</p></div>
  <form action="" method="post" class="formulario">
    <div class="item">
      <p>1 persona</p> <input type="radio" name="num_person" id="">
    </div>
    <div class="item">
      <p>2 personas</p> <input type="radio" name="num_person" id="">
    </div>
    <div class="item">
      <p>3 personas</p> <input type="radio" name="num_person" id="">
    </div>
    <div class="item">
      <p>4 personas</p> <input type="radio" name="num_person" id="">
    </div>
    <div class="item">
      <p>5 o mas personas</p> <input type="radio" name="num_person" id="">
    </div>
  </form>

  <div class="boton"><button @click="$router.push('/about')" class="btn">Continuar</button></div>

</template>

<script>
import HelloWorld from "@/components/HelloWorld.vue";
import Saludo from "@/components/Saludo.vue";
export default {
  components:{HelloWorld,Saludo}

}
</script>

<style lang="scss" scoped>
.pregunta{
  text-align: center;
  margin-top: 12%;
  font-size: 1.3rem;
}
.formulario{
  margin-top: 15%;
  .item{
    display: flex;
    justify-content: space-between;
    font-size: 1.5rem;
    margin-top: 5%;
  }
}
.boton{
  margin-top: 50%;
  text-align: center;
  height: 5vh;
  .btn{
    width: 50%;
    height: 80%;
    border-radius: 10px;
    border: none;
    background: black;
    color: white;
  }
}
</style>