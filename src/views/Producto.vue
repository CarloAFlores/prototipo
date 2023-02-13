<template>
    <HelloWorld/>

    <div class="contenedor">
        <img src="@/assets/rancheros.jpg" class="refencia">
        <div class="precio"><span>$$$$$</span></div>
    </div>

    <section class="descripcion">
        <p class="platillo">Hamburguesa de Pavo a la Parrila</p>
        <p class="descripcion">Hamburguesa de pechuga de pavo(80 g), espinacas,
        germinado y aguacate, acompanado con ensalada o 
        papas fritas.</p>
        <div class="extra_info">
            <img src="@/assets/info_circle.svg" alt="">
            <p>El gramaje se expresa en producto crudo de carnicos y varia de acuerdo a 
            su coccion</p>
        </div>

        <div class="iniciar_compra">
            <p>!Completa tu orden en tan solo 1 paso!</p>
            <div>
                <img src="" alt="">
                <p>!Elige la <span>guarnicion</span> que deseas y solicita tu pedido</p>
            </div>

        </div>
    </section>

    <section class="seleccion_guarni">
       <div class="ventana_1">

       </div>
       <div class="ventana_2">

       </div>
    </section>

</template>

<script>
import HelloWorld from "@/components/HelloWorld.vue";
import font from "@/common/font.css";
export default {
    components:{HelloWorld}

}
</script>

<style lang="scss" scoped>
.refencia{
    width: 100%;
}
.precio{
    background: orangered;
    color: white;
    text-align: center;
    position: absolute;
    width: 20%;
    top: 32%;
    right: 10%;
    border-radius: 15px;
}
.descripcion{
    background: goldenrod;
    font-family: AvenirLTStd-book;
    .platillo{
        font-weight: bold;
        margin-top: 10%;
    }
    .descripcion{
        margin-top: 8%;
    }
    .extra_info{
        display: flex;
        font-style: italic;
        font-size: 70%;
        margin-top: 5%;
    }

}
.seleccion_guarni{
    background: salmon;
}

</style>