<template>
<HelloWorld/>
<Saludo/>

<div class="div__p"><p>Cuantas personas se encuentra en tu mesa?</p></div>
<form action="" method="post" class="form">
  <div class="form__div">
    <p>1 persona</p>
    <input type="radio" name="num_person" id="">    
  </div>
  <div class="form__div">
    <p>2 personas</p>
    <input type="radio" name="num_person" id="">    
  </div>
  <div class="form__div">
    <p>3 personas</p>
    <input type="radio" name="num_person" id="">    
  </div>
  <div class="form__div">
    <p>4 personas</p>
    <input type="radio" name="num_person" id="">    
  </div>

  <div class="form__div">
    <p>5 o mas personas</p>
    <input type="radio" name="num_person" id="">    
  </div>
</form>

<div class="div">
  <button class="div__btn">Ir al menu</button>
</div>
  
</template>

<script>
import HelloWorld from "@/components/Header.vue";
import Saludo from "@/components/Saludo.vue";
export default {
  components:{HelloWorld,Saludo}

}
</script>

<style lang="scss" scoped>
.div__p{
  text-align: center;
  margin-top: 10%;
}
.form{
  margin-top: 8%;
  &__div{
  display: flex;
  justify-content: space-between;
  margin-top: 8%;
}
}
.div{
  margin-top: 60%;
  display: flex;
  justify-content: center;
  height: 5vh;
  &__btn{
    background: var(--negro);
    color: white;
    width: 60%;
    border-radius: 15px;
  }
}


</style>