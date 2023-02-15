<template>
<HelloWorld/>
<Saludo/>
<section class="buscador">
        <input type="text" name="" id="" class="buscador__input">
</section>

<section class="section">
    <div class="section__div">
        <h2 class="text">Para ti</h2>
        <p>Creamos sugerencias basadas en tus ultimos pedidos para ayudar a elegir</p>
        <Recomendacion/>
    </div>
</section>

<section class="section">
    <div class="section__div">
        <h2 class="text">Recomendaciones del chef</h2>
        <p>Las mejores delicias</p>
        <Sugerencia/>
    </div>
</section>

<section class="section">
    <div class="section__div">
        <h2 class="text">Promociones</h2>
        <p>Es momento de consentirse</p>
        <Promociones/>
    </div>
</section>

<section class="horario">
    <div class="horario__div div">
        <h2 class="div__text">Desayunos</h2>
        <p>Servicio de 8 a 12 horas</p>
    </div>
    <div class="horario__div div">
        <h2 class="div__text">Comidas</h2>
        <p>Servicio de 12 a 18 horas</p>
    </div>
    <div class="horario__div div">
        <h2 class="div__text">Cenas</h2>
        <p>Servicio de 18 a 20 horas</p>
    </div>

    <div class="opciones">
        <button class="opciones--click">Desayunos</button>
        <button class="opciones--click">Comidas</button>
        <button class="opciones--click">Cenas</button>
    </div>

    <div class="div__active">
        <Desayunos/>
    </div>
    <div class="div__active">
        <Comidas/>
    </div>
    <div class="div__active">
        <Cena/>
    </div>
</section>
  
</template>

<script>
import HelloWorld from "@/components/Header.vue";
import Saludo from "@/components/Saludo.vue";
import Recomendacion from "@/components/Recomendacion.vue";
import Sugerencia from "@/components/Sugerencia.vue";
import Promociones from "@/components/Promociones.vue";
import Desayunos from "@/components/Desayunos.vue";
import Comidas from "@/components/Comidas.vue";
import Cena from "@/components/Cena.vue";
export default {
    components:{HelloWorld,Saludo,Recomendacion,Sugerencia,Promociones,
    Desayunos,Comidas,Cena}

}
</script>

<style lang="scss" scoped>
.buscador{
    display: flex;
    justify-content: center;
    &__input{
        margin-top: 13%;
        height: 5vh;
        width: 80%;
        &[type=text]{
            width: 80%;
            border: none;
            border-radius: 8px;
            background:  rgba(177, 177, 177, 0.329);
            background-image: url('@/assets/search.svg');
            background-position: 10px 10px; 
            background-repeat: no-repeat;
            padding: 12px 20px 12px 40px;
        }
    }
}
.section{
    margin-top: 8%;
    display: flex;
    justify-content: center;
    &__div{
        width: 80%;
        .text{
            font-family: var(--tipo-tercearia);
        }
    }
}
.horario{
    margin-top: 15%;
    display: flex;
    align-items: center;
    flex-direction: column;
    &__div{
        width: 80%;
        &__text{
            font-family: var(--tipo-tercearia);
        }
    }
    .opciones{
        width: 80%;
        display: flex;
        &--click{
            width: 33.3%;
            &:focus{
                transition: all 0.2s ease-out;
                border-bottom: 5px solid orange;
                color: orange;
            }
        }
    }
    .div__active{
        width: 80%;
    }
}

</style>