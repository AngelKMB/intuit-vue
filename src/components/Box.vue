<template>
  <div class="box">
      <h2>{{ title }}</h2>
      <slot/>
  </div>
</template>

<script>
export default {
    name: 'Box',
    props: {
        title: {
            type: String,
            default: ''
        }
    },
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css?family=Josefin+Sans');

.box{
    padding: 40px;
    background-color: #eceef1;
    width: 80%;
}

h2 {
    font-family: 'Josefin Sans';
    font-weight: 600;
}
</style>