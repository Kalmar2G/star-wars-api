<template>
  <v-container class="wrapper">
    <div class="navigation">
      <router-link to="/">
        <my-button><span>Main</span>
        </my-button>
      </router-link>
      <router-link to="/characters">
        <my-button><span>Characters</span>
        </my-button>
      </router-link>
      <router-link to="/starships">
        <my-button><span>Starships</span></my-button>
      </router-link>
    </div>
  </v-container>
</template>

<script>
import MyButton from './MyButton.vue';

export default {
  components: {
    MyButton,
  },
};
</script>

<style scoped>
.wrapper {
  margin: 0 auto;
  max-width: 1000px;
}

.navigation {
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 100px;
  width: 100%;
}
</style>
