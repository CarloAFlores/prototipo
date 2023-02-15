<template>
  <Header/>

  <section class="section">
    <img src="@/assets/huevos.jpg" class="section__img">
    <div class="section__div"> <span>$ #####</span> </div>
  </section>

  <section class="informacion">
    <div class="informacion__div">
        <h3 class="informacion__div__h2">Hamburguesa de Pavo a la Parrilla</h3>
        <p class="informacion__div__p">Hamburguesa de pechuga de pavo (80g), espinacas,
            germinados y aguacate, acompanado con ensalada o papas fritas
        </p>
        <div class="informacion__div__informacion"><img src="@/assets/info_circle.svg" class="informacion__div__informacion__img"> 
        <p>El gramaje se expresa en producto crudo de carnicos y
            varia de acuerdo a su coccion </p></div>
    </div>

    <div class="informacion__div2">
        <h4 class="informacion__div2__h3">!Completa tu orden en tan solo 1 paso!</h4>
        <div class="informacion__div2__pasos">
            <img src="@/assets/circle.svg" class="informacion__div2__pasos__img">
            <p class="informacion__div2__pasos__p">!Elige la <strong> guarnicion </strong> que deseas y solicita tu pedido!</p>
        </div>
    </div>

    <div class="informacion__button">
        <button class="informacion__button__btn--click">Comenzar mi orden</button>
    </div>
  </section>
</template>

<script>
import Header from "@/components/Header.vue";
export default {
    components:{Header}

}
</script>

<style lang="scss" scoped>
.section{
    &__img{
        width: 100%;
    }
    &__div{
        position: absolute;
        top: 32%;
        left: 65%;
        background: orangered;
        color: var(--blanco );
        border-radius: 10px;
        width: 28%;
        text-align: center;
    }
}
.informacion{
    display: flex;
    flex-direction: column;
    align-items: center;
    &__div{
        width: 90%;
        margin-top: 8%;
        &__h2{
            font-family: var(--tipo-tercearia);
        }
        &__p{
            margin-top: 5%;
        }
        &__informacion{
            margin-top: 3%;
            font-family: var(--tipo-cuarta);
            font-size: 70%;
            display: flex;
            &__img{
                width: 8%;
                padding: 4px -1px 0px 5px;
            }
        }
    }
    &__div2{
        margin-top: 10%;
        width: 90%;
        &__h3{
            font-family: var(--tipo-tercearia);
        }
        &__pasos{
            margin-top: 7%;
            display: flex;
            &__img{
            width: 8%;
            padding: 4px -1px 0px 5px;
            }
            &__p{
                margin-left: 3%;
            }
        }

    }
    &__button{
        width: 90%;
        display: flex;
        justify-content: center;
        margin-top: 50%;
        &__btn--click{
            background: var(--negro);
            height: 5vh;
            width: 60%;
            border-radius: 10px;
            color: var(--blanco);
        }
    }
}


</style>