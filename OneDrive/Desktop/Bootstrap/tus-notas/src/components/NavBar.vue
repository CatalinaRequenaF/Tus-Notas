<template>
      <b-navbar toggleable="lg" class="navbar" type="dark">
        <b-navbar-brand class="title" to="/">Inicio</b-navbar-brand>
  
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
  
        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav class="flex">
            <b-nav-item to="/list">
              <img src="" alt="">
              Notas
            </b-nav-item>
            <b-nav-item to="/form">Añadir nota</b-nav-item>
            <b-nav-item to="/find">Buscar</b-nav-item>

          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
  </template>

<script>
    export default {
      name: "FormNota",
    }
    </script>
  
  <style>
  @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@600&family=Poppins:wght@400;500;600;700&display=swap');
  
    .title{
      font-weight: 600;
    }
  
    .navbar{
      background-color: #24922c;
      box-shadow: 0px 1px 5px -2px rgba(0,0,0,0.45);
    -webkit-box-shadow: 0px 1px 5px -2px rgba(0,0,0,0.45);
    }
  </style>
  