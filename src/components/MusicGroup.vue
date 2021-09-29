<template>
  <div class="music-container container">
    <div class="row d-flex">
      
      <div v-for="(music, index) in musicList" :key="index" 
      class="music-card img-fluid">
        <MusicCard :musicItem="music"/>
      </div>

    </div>
  </div>
</template>

<script>
import axios from "axios";
import MusicCard from "./MusicCard.vue";

export default {
  name: 'MusicGroup',
  props: {
    msg: String
  },
  data : function () {
    return{
      musicList : []
    }
  },
   components:{
    MusicCard,
  },
  mounted() {

    axios.get("https://flynn.boolean.careers/exercises/api/array/music")
    .then((risposta) =>{
      
      this.musicList = risposta.data.response.slice();
      console.log(this.musicList);
    })
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../style/general.scss";
@import "../style/variabiles.scss";

.music-card{
  width: calc(100% / 5);
  
}

</style>
