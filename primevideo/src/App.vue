<template>
<div id="app">
    <nav class="navbar">
      <div class="links">
       <div class="left">
         <div>
           <img src="./assets/logo.png" width="220px">
         </div>
         <div>
           <input class="btn" type="button" value="Início">
           <input class="btn" type="button" value="Séries">
            <input class="btn" type="button" value="Filmes">
           <input class="btn" type="button" value="Infantil">
          <input class="btn" type="button" value="Canais">
         </div> 
       </div>
      <div class="right">    
        <form>
          <input
          type="search"
          class="Search"
          placeholder="Busca">
          <img src="./assets/magnifiying-glass.png" alt="">
        </form>
      <div class="User">
         <img
            src="https://icon-icons.com/icons2/2760/PNG/32/profile_icon_176363.png"
           alt="User">
      </div>
    </div>
   </div>
  </nav>

   <Menu />

    <footer class="footer">
      <div class="fimg">
          <img src="./assets/logo.png" width="200px">
      </div>
      <div class="f1">
        <li>
          <a href="#">Termos e aviso de privacidade</a>
        </li>
        <li>
          <a href="#">Enviar feedback</a>
          </li>
        <li>
          <a href="#">Ajuda</a>
          </li>
          <div>
            <li>© 1996-2021, Amazon.com, Inc. ou suas afiliadas</li>
          </div>
      </div>
    </footer>
  </div>
</template>

<script>
import Menu from './components/Menu';

export default {
  name: 'App',

  components: {
   Menu,
  }
};
</script>

<style>
body {
  padding: 0px;
  margin: 0px;
  font-family:Arial, Helvetica, sans-serif
}

#app {
  display: grid;
  grid-template-areas: "nav" ;
  grid-template-rows: 11.5vh;
}

.navbar {
  grid-area: nav;
  background-color: #1e2735;
}
.links{
  display: flex;
  padding: 27px;
  flex-direction: row;
  justify-content: space-between;
}
.btn {
  padding: 12px;
  font-size: 25px;
  border: none;
  outline: none;
  cursor: pointer;
  color: rgb(199, 199, 199);
  background-color: transparent;
}
.Search {
  padding: 12px;
  font-size: 25px;
  cursor: pointer;
  outline: none;
  border-color: rgb(199, 199, 199) ;
  color: rgb(199, 199, 199);
  background-color: #1a222e;
}
.User {
  font-size: 30px;
  padding: 12px;
  color: rgb(199, 199, 199);
}
.footer {
  font-size: 22px;
  padding: 12px;
  color: rgb(146, 145, 145);
  list-style: none;
}
.left {
  display: flex;
  justify-items: center;
  flex-direction: row;
}
.right {
  display: flex;
  justify-items: center;
  flex-direction: row;
}
.fimg {
  display: flex;
  justify-content: center;
  padding-top: 50px;
  margin: 10px;
}
.f1 {
  display: flex;
  justify-content: center;
}
.f1 li a{
  margin-left: 0px;
  text-decoration: none;
  color: rgba(148, 215, 253, 0.733);
}
.f1 li {
  margin-left: 22px;
}
</style>