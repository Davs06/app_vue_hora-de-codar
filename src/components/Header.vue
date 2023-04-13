<template>
  <div>
    <header>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Projetos</a></li>
        <li><a href="#">Sobre</a></li>
      </ul>
    </header>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<!-- scoped css -- manipula o estilo do componente -->

<style scoped>
header{
    background-color: #999;
    margin: 0;
    padding: 10px;
}

ul{
    display: flex;
}

li{
    list-style: none;
    margin: 0 5px;
}

a{
    text-decoration: none;
    transition:.5s;
}

a:hover{
    transform: scale(1.2px);
    color: aqua;
}

</style>