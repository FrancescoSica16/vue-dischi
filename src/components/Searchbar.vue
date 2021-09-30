<template>
 <div class="check-genere">
    <input type="checkbox" id="genere" :name="genreSelected.genre" :value="genreSelected.genre">
    <label for="genere">{{genreSelected.genre}}</label>
  </div> 

</template>

<script>
export default {
    name: "Searchbar",  
    props: ["genreSelected"],

    data : function () {
        return{
          genre: "",
        }
    },

    computed:{

    },

    mounted:{

    },
    methods:{

    }
}
</script>

<style lang="scss" scoped>
@import "../style/general.scss";
@import "../style/variabiles.scss";

.check-genere{
  padding: 10px;
  color: white;
}

</style>