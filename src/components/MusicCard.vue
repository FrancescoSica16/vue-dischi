<template>
  <div class="music-card-wrapper">
      <img class="img-fluid" :src="musicItem.poster" alt="">
      <h5 class="titolo">{{musicItem.title}}</h5>
      <p class="author">{{musicItem.author}}</p>    
      <p class="year">{{musicItem.year}}</p>  
  </div>
</template>

<script>

export default {

name: "MusicCard",
props: ["musicItem"],

}
</script>

<style lang="scss" >
@import "../style/general.scss";
@import "../style/variabiles.scss";

    .music-card-wrapper{
        text-align: center;
        min-height: 280px ;
        margin: 10px 0;
        background-color: $background-color;
        padding: 10px;

        img{
            margin-bottom: 10px;
        }
        h5{
            color: $titol-color;
        }

        p{
            color: $sub-color;

          
        }

    }
</style>