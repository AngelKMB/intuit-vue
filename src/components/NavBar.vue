<template>
    <nav>
      <ul>
          <li class="push-left"> <router-link to="/"><img alt="Quickbooks logo" width="155px" src="@/assets/logo-quickbooks.png"></router-link></li>
          <li><router-link to="/item1">Item 1</router-link></li>
          <li><router-link to="/item2">Item 2</router-link></li>
      </ul>
    </nav>
</template>

<script>
export default {
    name: 'NavBar'
}
</script>

<style scoped>

nav ul {
  display: flex;
  justify-items: end;
}

nav li {
    margin: 0 10px;
    list-style: none;
}

.push-left {
  margin-right: auto;
}

a {
  color: #000;
  text-decoration: none;
  font-weight: 200;
}

</style>