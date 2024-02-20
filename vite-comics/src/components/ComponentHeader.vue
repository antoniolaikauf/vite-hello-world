<script>
export default {
  name: " ComHeader",


  data() {
    return {
      // array con feat della pagina 
      links: [
        {
          text:"CHARACTERS",
          url:"#",
          current:false,
        },
        {
          text:"COMICS",
          url:"#",
          current:true,
        },
        {
          text:"MOVIES",
          url:"#",
          current:false,
        },
        {
          text:"TV",
          url:"#",
          current:false,
        },
        {
          text:"GAMES",
          url:"#",
          current:false,
        },
        {
          text:"COLLECTIBLES",
          url:"#",
          current:false,
        },
        {
          text:"VIDEOS",
          url:"#",
          current:false,
        },
        {
          text:"FANS",
          url:"#",
          current:false,
        },
        {
          text:"NEWS",
          url:"#",
          current:false,
        },
        {
          text:"SHOP",
          url:"#",
          current:false,
        },
      ]
    }
  }
}

</script>

<template>
  <header class="sfondo">
    <nav class="display-menu">
      <!-- immagine logo -->
      <div>
        <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <!-- lista menu -->
      <ul>
        <li v-for="link in links">
          <a :href="link.url" :class="{active:link.current}">{{ link.text }}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<style scoped lang="scss">
@use '../style/general.scss' as *;
@use '../style/partials/variable' as *;

.display-menu {
  // caratteristiche generali di nav 
  display: $display_flex ;
  justify-content: $specific_content;
  width: $width_blocchi;
  margin: $margin_blocchi;
  align-items: $specific_align;
  height: 100px;

  img {
    width: 60px;
  }
// caratteristiche di ul e i tag al suo interno 
  ul {
    display: $display_flex ;
    height: 100%;

    a {
      padding: 0px 10px;
      display: $display_flex ;
      align-items: $specific_align;
      height: 100%;
    }

  }

// classe per capire pagina attuale 
  .active{
    color: $color-bg;
    border-bottom: 2px solid $color-bg;
  }
}
</style>
