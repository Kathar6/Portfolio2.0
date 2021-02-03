<template>
  <div class="nav">
    <ul>
      <li><router-link to="/">Home</router-link></li>
      <li><router-link to="/about">About</router-link></li>
      <li><router-link to="/contact">Contact</router-link></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Nav",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.nav{
  color:#afafaf;
  font-size: 1.2em;
  & a {
    all: unset;
  }
  & a:visited {
    color: #afafaf;
  }
  & li {
    display: inline-block;
    margin: 0 10px;
    border-bottom: 3px solid #c8c8c8;
    cursor: pointer;
    transition-property: color, border-bottom-color;
    transition: .5s;
  }
  & a:hover, li:hover{
    color: #000;
    border-bottom-color: #1e88e5;
  }
}
ul {
  list-style-type: none;
  padding: 0;
  margin: 2% 0;
}

</style>
