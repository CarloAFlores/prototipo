<template>
  <section class="comida">
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
    <div class="items"><router-link :to="{name:'seleccion'}">Grid item12</router-link></div>
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
.comida{
    display: grid;
    grid-template-columns: repeat(aut-fit,auto);
    gap: .5rem;
    .items:nth-child(1){
        background: palevioletred;
        grid-column: span 2;
    }
    .items:nth-child(12){
        background: palevioletred;
        grid-column: span 2;
    }
}

</style>