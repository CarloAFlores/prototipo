<template>
  <section class="section">
    <img src="@/assets/rancheros.jpg" class="section__img">
    <button class="section__btn"><img src="@/assets/arrow_return.svg" alt=""></button>
    <div class="section__div"><p>Huevos y Omelettes</p></div>
  </section>


  <section class="promociones">
    <div class="promociones__div">
      <button class="promociones__div__btn--click">Promociones</button>
      <button class="promociones__div__btn--click">Recomendados para ti</button>
    </div>

    <div class="promociones__component"><Recomendacion/></div>
    <!-- <div class="promociones__component"><Promociones/></div> -->
  </section>

  <section class="informacion">
    <div class="informacion__div">
      <h2 class="informacion__div__h2">Huevos y Omelettes</h2>

      <div class="informacion__div__horario"><p>Servido de lunes a viernes de 7 a 12 horas,
        sabado y domingos hasta las 13 horas </p></div>

      <span class="informacion__div__span">Todos los huevos y omelettes incluyen 
      <b class="informacion__div__span__b">fruta</b> + <b class="informacion__div__span__b">cafe americano</b>
       o  <b class="informacion__div__span__b"> te caliente </b> 
      </span>
    </div>
  </section>

  <section class="platillo">
    <div class="platillo__div">
      <img src="@/assets/logo.png" class="platillo__div__img">
      <div class="platillo__div__informacion">
        <div class="platillo__div__informacion__div"><p>Huevos al gusto</p>
        <button class="platillo__div__informacion__div__btn">$####</button></div>

        <div class="platillo__div__informacion__div2">
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>
      </div>
    </div>

    <div class="platillo__div">
      <img src="@/assets/logo.png" class="platillo__div__img">
      <div class="platillo__div__informacion">
        <div class="platillo__div__informacion__div"><p>Huevos al gusto</p>
        <button class="platillo__div__informacion__div__btn">$####</button></div>

        <div class="platillo__div__informacion__div2">
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>
      </div>
    </div>

    <div class="platillo__div">
      <img src="@/assets/logo.png" class="platillo__div__img">
      <div class="platillo__div__informacion">
        <div class="platillo__div__informacion__div"><p>Huevos al gusto</p>
        <button class="platillo__div__informacion__div__btn">$####</button></div>

        <div class="platillo__div__informacion__div2">
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>
      </div>
    </div>

    <div class="platillo__div">
      <img src="@/assets/logo.png" class="platillo__div__img">
      <div class="platillo__div__informacion">
        <div class="platillo__div__informacion__div"><p>Huevos al gusto</p>
        <button class="platillo__div__informacion__div__btn">$####</button></div>

        <div class="platillo__div__informacion__div2">
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>
      </div>
    </div>

    <div class="platillo__div">
      <img src="@/assets/logo.png" class="platillo__div__img">
      <div class="platillo__div__informacion">
        <div class="platillo__div__informacion__div"><p>Huevos al gusto</p>
        <button class="platillo__div__informacion__div__btn">$####</button></div>

        <div class="platillo__div__informacion__div2">
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>
      </div>
    </div>

    <div class="platillo__div">
      <img src="@/assets/logo.png" class="platillo__div__img">
      <div class="platillo__div__informacion">
        <div class="platillo__div__informacion__div"><p>Huevos al gusto</p>
        <button class="platillo__div__informacion__div__btn">$####</button></div>

        <div class="platillo__div__informacion__div2">
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>
      </div>
    </div>
  </section>


</template>

<script>
import Recomendacion from "@/components/Recomendacion.vue";
import Promociones from "@/components/Promociones.vue";
export default {
  components:{Recomendacion,Promociones}

}
</script>

<style lang="scss" scoped>
.section{
  position: relative;
  &::before{
    background: rgba(0,0,0,.4);
    width: 100%;
    height: 100%;
    position: absolute;
    content: "";
  }
  &__btn{
    position: absolute;
    left: 6%;
    top: 45%;
    background: transparent;
  }
  &__div{
    position: absolute;
    left: 15%;
    top: 42%;
    color: var(--blanco);
    font-size: 1.8rem;
    font-family: var(--tipo-tercearia);
  }
}
.promociones{
    margin-top: 8%;
    display: flex;
    flex-direction: column;
    align-items: center;
    &__div{
      display: flex;
      width: 92%;
      &__btn--click{
        margin-left: 1rem;
        &:focus{
          transition: all 0.2s ease-out;
          border-bottom: 1.5px solid orange;
          color: orange;
        }
      }
    }
    &__component{
      width: 92%;
    }
  }
.informacion{
  margin-top: 10%;
  display: flex;
  justify-content: center;
  &__div{
    width: 92%;
    &__h2{
      font-family: var(--tipo-tercearia );
    }
    &__horario{
      margin-top: 5%;
      margin-bottom: 5%;
      display: flex;
      align-items: center;
      height: 8vh;
      border-radius: 8px;
      background: rgba(248, 186, 72, 0.363);
      border: 1px solid rgb(255, 81, 0);
    }
    &__span{
      &__b{
        font-family: var(--tipo-tercearia);
      }
    }
  }
}
.platillo{
  margin-top: 10%;
  display: flex;
  flex-direction: column;
  align-items: center;
  &__div{
    margin-top: 8%;
    width: 92%;
    display: flex;
    box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
    &__img{
      width: 40%;
    }
    &__informacion{
      width: 100%;
      display: flex;
      flex-direction: column;
      align-items: center;
      &__div{
        margin-top: 7%;
        width: 95%;
        display: flex;
        justify-content: space-between;
        &__btn{
          width: 35%;
          border-radius: 10px;
          background: orange;
          color: var(--blanco );
        }
      }
      &__div2{
        margin-top: 8%;
        width: 95%;
      }
    }
  }
}

</style>