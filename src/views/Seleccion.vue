<template>
  <div class="contendor">
    <img src="@/assets/huevos.jpg" class="logo" />
    <button @click="this.$router.go(-1)" class="return">
      <img src="@/assets/arrow_return.svg" class="flecha" />
    </button>
    <div class="titulo">Huevos y Omelette</div>
  </div>

  <div class="botones">
    <button class="btn_item" @click="showAbrir('1')">Promociones</button>
    <button class="btn_item" @click="showAbrir('2')">Recomendado para ti</button>
  </div>

  <div v-if="abrir"><Recomendacion/></div>
  <div v-if="abrir2"><Promociones/></div>

  <section class="datos">
    <p class="titulo_dos">Huevos y Omelettes</p>
    <div class="horario">
      <p>
        Servidos de lunes a viernes de 7 a 12 horas y 
        sabados y domingos hasta las 13 horas
      </p>
    </div>

    <div class="reglas">
      <p>
        Todos los huevos y omelettes incluyen jugo o fruta + cafe 
        americano o te caliente
        <button class="vermas"><img src="@/assets/info.svg" /></button>
      </p>
    </div>
  </section>

  <section class="productos">

    <div class="categoria">Huevos y omelettes</div>

    <div class="platillo" @click="$router.push({name:'producto', query:{huevos:'num_1'}})">
      <img src="@/assets/logo.png" class="imagen_plati" />
      <div class="informacion">
        <div class="precio">
          <p>Huevos al gusto</p>
          <span class="dinero">$$$$$</span>
        </div>
        <p class="descripcion">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Rem commodi
          tempora doloribus fugiat eligendi explicabo quod
        </p>
      </div>
    </div>
    <div class="platillo" @click="$router.push({name:'producto', query:{huevos:'num_2'}})">
      <img src="@/assets/logo.png" class="imagen_plati" />
      <div class="informacion">
        <div class="precio">
          <p>Huevos al gusto</p>
          <span class="dinero">$$$$$</span>
        </div>
        <p class="descripcion">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Rem commodi
          tempora doloribus fugiat eligendi explicabo quod
        </p>
      </div>
    </div>
    <div class="platillo" @click="$router.push({name:'producto', query:{huevos:'num_3'}})">
      <img src="@/assets/logo.png" class="imagen_plati" />
      <div class="informacion">
        <div class="precio">
          <p>Huevos al gusto</p>
          <span class="dinero">$$$$$</span>
        </div>
        <p class="descripcion">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Rem commodi
          tempora doloribus fugiat eligendi explicabo quod
        </p>
      </div>
    </div>
    <div class="platillo" @click="$router.push({name:'producto', query:{huevos:'num_4'}})">
      <img src="@/assets/logo.png" class="imagen_plati" />
      <div class="informacion">
        <div class="precio">
          <p>Huevos al gusto</p>
          <span class="dinero">$$$$$</span>
        </div>
        <p class="descripcion">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Rem commodi
          tempora doloribus fugiat eligendi explicabo quod
        </p>
      </div>
    </div>
    <div class="platillo" @click="$router.push({name:'producto', query:{huevos:'num_5'}})">
      <img src="@/assets/logo.png" class="imagen_plati" />
      <div class="informacion">
        <div class="precio">
          <p>Huevos al gusto</p>
          <span class="dinero">$$$$$</span>
        </div>
        <p class="descripcion">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Rem commodi
          tempora doloribus fugiat eligendi explicabo quod
        </p>
      </div>
    </div>
    <div class="platillo" @click="$router.push({name:'producto', query:{huevos:'num_5'}})">
      <img src="@/assets/logo.png" class="imagen_plati" />
      <div class="informacion">
        <div class="precio">
          <p>Huevos al gusto</p>
          <span class="dinero">$$$$$</span>
        </div>
        <p class="descripcion">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Rem commodi
          tempora doloribus fugiat eligendi explicabo quod
        </p>
      </div>
    </div>
    <div class="platillo">
      <img src="@/assets/logo.png" class="imagen_plati" />
      <div class="informacion">
        <div class="precio">
          <p>Huevos al gusto</p>
          <span class="dinero">$$$$$</span>
        </div>
        <p class="descripcion">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Rem commodi
          tempora doloribus fugiat eligendi explicabo quod
        </p>
      </div>
    </div>
    <div class="platillo">
      <img src="@/assets/logo.png" class="imagen_plati" />
      <div class="informacion">
        <div class="precio">
          <p>Huevos al gusto</p>
          <span class="dinero">$$$$$</span>
        </div>
        <p class="descripcion">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Rem commodi
          tempora doloribus fugiat eligendi explicabo quod
        </p>
      </div>
    </div>
    <div class="platillo">
      <img src="@/assets/logo.png" class="imagen_plati" />
      <div class="informacion">
        <div class="precio">
          <p>Huevos al gusto</p>
          <span class="dinero">$$$$$</span>
        </div>
        <p class="descripcion">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Rem commodi
          tempora doloribus fugiat eligendi explicabo quod
        </p>
      </div>
    </div>
    <div class="platillo">
      <img src="@/assets/logo.png" class="imagen_plati" />
      <div class="informacion">
        <div class="precio">
          <p>Huevos al gusto</p>
          <span class="dinero">$$$$$</span>
        </div>
        <p class="descripcion">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Rem commodi
          tempora doloribus fugiat eligendi explicabo quod
        </p>
      </div>
    </div>
  </section>
</template>

<script>
import { ref } from '@vue/reactivity';
import Recomendacion from "@/components/Recomendacion.vue";
import Promociones from "@/components/Promociones.vue";
export default {
  components:{Recomendacion,Promociones},
      setup(){
        const abrir = ref(true)
        const abrir2 = ref(false)
        const abrir3= ref(false)

        const showAbrir = ((showAbrir)=>{

            if(showAbrir == '1'){
                abrir2.value=false
                abrir3.value=false
                return abrir.value=true
            }if(showAbrir == '2'){
                abrir.value=false
                abrir3.value=false
                return abrir2.value=true
            }if(showAbrir =='3'){
                abrir.value=false
            abrir2.value=false
            return abrir3.value=true
            }
        })
        return{
            showAbrir,
            abrir,
            abrir2,
            abrir3
        }
    }
};
</script>

<style lang="scss" scoped>
.contendor {
  width: 100%;
  position: relative;
  &.contendor::before {
    background-color: rgba(0, 0, 0, 0.5);
    width: 100%;
    height: 100%;
    position: absolute;
    content: "";
  }
  .logo {
    width: 100%;
  }
  .return {
    position: absolute;
    left: 6%;
    top: 45%;
    background: transparent;
    border: none;
    .flecha {
      width: 100%;
    }
  }
  .titulo {
    position: absolute;
    left: 15%;
    top: 42%;
    font-size: 2rem;
    font-weight: bold;
    color: white;
    font-family: AvenirLTStd-book;
  }
}
.botones {
  .btn_item {
    width: 41%;
    height: 5vh;
    background: white;
    border: none;
    transition: all 0.5s ease-out;
    font-size: 1rem;

    &:focus {
      transition: all 0.2s ease-out;
      border-bottom: 5px solid orange;
      color: orange;
    }
  }
}
.datos {

  font-family: AvenirLTStd-book;
  .titulo_dos {
    font-weight: bold;
    font-size: 1.3rem;
  }
  .horario {
    margin-top: 5%;
    border: 1px solid orangered;
    border-radius: 10px;
    background: rgb(255, 192, 74);
    font-size: 1.2rem;
    height: 10vh;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .reglas {
    margin-top: 5%;
    width: 100%;
    .vermas {
      background: transparent;
      border: none;
    }
  }
}
.productos {

  display: flex;
  flex-direction: column;
  .categoria{
    font-size: 1.5rem;
    font-weight: bold;
    font-family: AvenirLTStd-book;
  }
  .platillo {

    display: flex;
    box-shadow: 0px 5px #88888893;
    margin-top: 1rem;
    font-family: AvenirLTStd-book;
    .imagen_plati {
      width: 30%;
    }
    .informacion {
      width: 100%;
      .precio {
        display: flex;
        justify-content: space-around;
        .dinero {
          text-align: center;
          width: 30%;
          background: orangered;
          color: white;
          border-radius: 15px;
        }
      }
      .descripcion {
        margin-top: 3%;
        font-weight: lighter;
        color: rgb(156, 152, 152);
      }
    }
  }
}
</style>