<template>
<HelloWorld/>
<Saludo/>

<div class="block_saludo"><p>Cuantas personas se encuentra en tu mesa?</p></div>
<form action="" method="post" class="form">
  <div class="form__block">
    <p>1 persona</p>
    <input type="radio" name="num_person" id="">    
  </div>
  <div class="form__block">
    <p>2 personas</p>
    <input type="radio" name="num_person" id="">    
  </div>
  <div class="form__block">
    <p>3 personas</p>
    <input type="radio" name="num_person" id="">    
  </div>
  <div class="form__block">
    <p>4 personas</p>
    <input type="radio" name="num_person" id="">    
  </div>

  <div class="form__block">
    <p>5 o mas personas</p>
    <input type="radio" name="num_person" id="">    
  </div>
</form>

<div class="btn">
  <button class="btn_continue">Ir al menu</button>
</div>
  
</template>

<script>
import HelloWorld from "@/components/HelloWorld.vue";
import Saludo from "@/components/Saludo.vue";
export default {
  components:{HelloWorld,Saludo}

}
</script>

<style lang="scss" scoped>
.block_saludo{
  text-align: center;
  margin-top: 10%;
}
.form{
  margin-top: 8%;
  .form__block{
  display: flex;
  justify-content: space-between;
  margin-top: 8%;
}
}
.btn{
  margin-top: 60%;
  display: flex;
  justify-content: center;
  height: 5vh;
  .btn_continue{
    background: var(--negro);
    color: white;
    width: 60%;
    border-radius: 15px;
  }
}


</style>