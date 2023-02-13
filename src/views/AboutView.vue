<template>
    <HelloWorld/>
    <Saludo/>

    <div class="buscador"> a</div>

    <section class="sugerencia">
        <p class="titulo">Sugerencia para ti</p>
        <p>Creamos sugerencias basadas en tus ultimos pedidos 
        para ayudarte a elegir </p>
        <Sugerencia/>
    </section>

    <section class="recomendacion">
        <p class="titulo">Recomendacion del Chef</p>
        <p>Las mejores delicias</p>
        <Recomendacion/>
    </section>

    <section class="promociones">
        <p class="titulo">Promociones</p>
        <p>Es momento de consentirse</p>
        <Promociones/>
    </section>

    <section class="seleccion">
        <div class="botones">
            <button class="btn_item" @click="showAbrir('1')">Desayuno</button>
            <button class="btn_item" @click="showAbrir('2')">Comida</button>
            <button class="btn_item" @click="showAbrir('3')">Cena</button>
        </div>
    </section>

   <div class="desayuno" v-if="abrir"><Desayunos/></div>
    <div class="comida" v-if="abrir2"><Comidas/></div>
    <div class="cena" v-if="abrir3"><Cena/></div>
  
</template>

<script>
import HelloWorld from "@/components/HelloWorld.vue";
import Saludo from "@/components/Saludo.vue";
import Sugerencia from "@/components/Sugerencia.vue";
import Recomendacion from "@/components/Recomendacion.vue";
import Promociones from "@/components/Promociones.vue";
import Desayunos from "@/components/Desayunos.vue";
import Comidas from "@/components/Comidas.vue";
import Cena from "@/components/Cena.vue";
import { ref } from '@vue/reactivity';
export default {
    components:{HelloWorld,Saludo,Sugerencia,Recomendacion,
    Promociones,Desayunos,Comidas,Cena},
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
}
</script>

<style lang="scss" scoped>
.buscador{
    background: hotpink;
    margin-top: 15%;
}

.sugerencia{
    margin-top: 10%;
    font-family: AvenirLTStd-book;
    .titulo{
        font-size: 1.5rem;
        font-weight: bold;
    }
}
.recomendacion{
    margin-top: 10%;
    font-family: AvenirLTStd-book;
    .titulo{
        font-size: 1.5rem;
        font-weight: bold;
    }
}
.promociones{
    margin-top: 10%;
    font-family: AvenirLTStd-book;
    .titulo{
        font-size: 1.5rem;
        font-weight: bold;
    }
}
.seleccion{
    margin-top: 2rem;
    .botones{
        .btn_item{
            width: 33.3%;
            height: 5vh;
            background: white;
            border: none;
            transition: all 0.5s ease-out;
            font-size: 1rem;

            &:focus{
                transition: all 0.2s ease-out;
                border-bottom: 5px solid orange;
                color: orange;
            }
        }
    }
}
</style>