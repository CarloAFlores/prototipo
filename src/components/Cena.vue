<template>
  <section class="cena">
    <div class="items"><router-link :to="{name:'seleccion'}">Grid item1</router-link></div>
    <div class="items"><router-link :to="{name:'seleccion'}">Grid item2</router-link></div>
    <div class="items"><router-link :to="{name:'seleccion'}">Grid item3</router-link></div>
    <div class="items"><router-link :to="{name:'seleccion'}">Grid item4</router-link></div>
    <div class="items"><router-link :to="{name:'seleccion'}">Grid item5</router-link></div>
    <div class="items"><router-link :to="{name:'seleccion'}">Grid item6</router-link></div>
    <div class="items"><router-link :to="{name:'seleccion'}">Grid item7</router-link></div>
    <div class="items"><router-link :to="{name:'seleccion'}">Grid item8</router-link></div>
    <div class="items"><router-link :to="{name:'seleccion'}">Grid item9</router-link></div>
    <div class="items"><router-link :to="{name:'seleccion'}">Grid item10</router-link></div>
    <div class="items"><router-link :to="{name:'seleccion'}">Grid item11</router-link></div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.items{
  padding: 1rem;
  font-size: 1.25rem;
  background-color: #666;
}
.cena{
    display: grid;
    grid-template-columns: repeat(aut-fit,auto);
    gap: .5rem;
    .items:nth-child(1){
        background: rgb(17, 70, 216);
        grid-column: span 3;
    }
    .items:nth-child(2){
        background: rgb(17, 70, 216);
        grid-column: span 3;
    }
    .items:nth-child(3){
        background: rgb(17, 70, 216);
        grid-column: span 2;
    }
    .items:nth-child(6){
        background: rgb(17, 70, 216);
        grid-column: span 2;
    }
    .items:nth-child(7){
        background: rgb(17, 70, 216);
        grid-column: span 2;
    }
    .items:nth-child(10){
        background: rgb(17, 70, 216);
        grid-column: span 2;
    }
    .items:nth-child(11){
        background: rgb(17, 70, 216);
        grid-column: span 3;
    }
}

</style>