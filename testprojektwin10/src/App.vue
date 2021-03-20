<template>
  
  <div id="app">
    <h1 align="center" class="header">Nils Dambowy</h1>
    <ul align="center">
      <li v-for="topic in menu" :key="topic.id"
       class="animate__animated animate__bounce listEl"> 
        {{topic.content}}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'App',
  data: () => ({
    menu:[
      {id:1, content:"Space1"},
      {id:2, content:"Space2"},
      {id:3, content:"Space3"},
      {id:4, content:"Space4"}
    ]
  })
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
  margin-top: 30px;
}

body{
  background-color: rgba(76, 201, 218, 0.589);
}

.header{
  color:white;
  text-decoration: underline;
  font-size: 3rem;
  text-shadow: 0 0 5px black;
}

.listEl{
  display:inline-block;
  font-family:monospace;
  font-size: 2rem;
  color:white;
  padding: 40px;
  animation: bounce;
  animation-duration: 2s;
  position:relative;
  margin-top: -30px;
}

</style>
