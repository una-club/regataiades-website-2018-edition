<template>
  <div id="app">
    <!-- i18n text -->
    <small>{{ $t("message.welcome") }}</small>
    <div>
      <!-- selector -->
      <select v-model="$i18n.locale">
        <option value="en">EN</option>
        <option value="fr">FR</option>
      </select>
    </div>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
