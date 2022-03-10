<template>
    <header class="header">
        <div class="container">
            <a href="#" class="header__logo">LOGO</a>
            <div class="header__links">
                <a href="#"><img src="@/assets/person.svg" alt="" /></a>
                <a href="#"><img src="@/assets/favorite.svg" alt="" /></a>
                <a href="#"><img src="@/assets/bag.svg" alt="" /></a>
                <button v-on:click="menuOpen = true" class="icon-menu"><img src="@/assets/menu.svg" alt="" /></button>
            </div>
        </div>    
    </header>
</template>
<script>
export default {
  name: 'AppHeader',
  data: () => {
      return {
        menuOpen: false
      }
  }
   
}
</script>
<style lang="scss">

@import '@/assets/common.scss';

.header {
    padding: 10px 0;
    box-shadow: 0 4px 4px rgba(0, 0, 0, 0.1);
    &__logo {
        color: $color-black;
        line-height: 1;
        font-size: 22px;
        font-weight: 700;
        text-decoration: none;
    }
    &__links {
        float: right;
        display: flex;
        a {
           margin: 0 10px; 
        }
        .icon-menu {
            display: none;
            background: none;
            border: none;
            margin-left: 10px;
            cursor: pointer;
            @include respond-to(mobile) { 
                display: block;
            }
        }
    }

}
</style>