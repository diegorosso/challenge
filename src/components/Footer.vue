<template>
    <div class="contra-footer" @click="scrollToTop">
      <ion-icon class="icono-class" name="chevron-up-outline"></ion-icon>
    </div>
  </template>
  
  <script>
  export default {
    methods: {
      scrollToTop() {
        window.scrollTo({
          top: 0,
          behavior: "smooth" // Hace el desplazamiento suave
        });
      }
    }
  };
  </script>
  
  <style scoped>
  .contra-footer {
    width: 100%;
    display: flex;
    justify-content: flex-end; /* Ajusté a flex-end en lugar de end */
    background-color: var(--raisin-black);
    cursor: pointer; /* Hace que el cursor se convierta en un puntero al pasar sobre el icono */
  }
  .icono-class {
    font-size: 3rem;
    padding: 2rem;
    color: var(--white);
    background-color: var(--raisin-black);
  }
  </style>
  