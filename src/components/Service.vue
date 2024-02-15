<template>
  <section style="margin-bottom: 5rem">
    <!-- div1 -->

    <div class="container">
      <div class="Hola">
        <h1 class="title-class">Main Service Offering</h1>

        <p class="text-class">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Fugiat
          laudantium repellat voluptates fugit est deserunt inventore autem
          labore eum dolorum. Lorem ipsum dolor sit amet consectetur adipisicing
          elit. Aliquam, libero.
        </p>

        <button class="btn btn-secondary">Lorem, ipsum.</button>
      </div>
      <div class="Hola2">
        <div class="display-end">
          <img class="imagen-class" src="../assets/Imagenes/dna.jpg" alt="" />
        </div>
      </div>
    </div>
    <!-- div2 -->
    <div class="container">
      <div class="Hola">
        <h1 class="title-class">Main Service Offering</h1>

        <p class="text-class">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Fugiat
          laudantium repellat voluptates fugit est deserunt inventore autem
          labore eum dolorum. Lorem ipsum dolor sit amet consectetur adipisicing
          elit. Aliquam, libero.
        </p>

        <button class="btn btn-secondary">Lorem, ipsum.</button>
      </div>
      <div class="Hola2">
        <div class="display-end">
          <img class="imagen-class" src="../assets/Imagenes/dna2.jpg" alt="" />
        </div>
      </div>
    </div>
    <!-- div3 -->
    <div class="container">
      <div class="Hola">
        <h1 class="title-class">Main Service Offering</h1>

        <p class="text-class">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Fugiat
          laudantium repellat voluptates fugit est deserunt inventore autem
          labore eum dolorum. Lorem ipsum dolor sit amet consectetur adipisicing
          elit. Aliquam, libero.
        </p>

        <button class="btn btn-secondary">Lorem, ipsum.</button>
      </div>
      <div class="Hola2">
        <div class="display-end">
          <img class="imagen-class" src="../assets/Imagenes/dna3.jpg" alt="" />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.title-class {
  font-size: var(--fs-1);
  margin-bottom: 2rem;
  color:#799BC8
}
.text-class {
  font-size: var(--fs-5);
  margin-bottom: 2rem;
  color:#799BC8
}
.imagen-class {
  width: 100%;
  margin-bottom: 2rem;
}
.container {
  padding: 10px;
}
@media (max-width: 600px) {
  .btn {
    margin-bottom: 2rem;
  }
}
@media (min-width: 601px) and (max-width: 1024px) {
  .container {
    display: flex;
    padding-inline: 16px;
  }
  .imagen-class {
    margin-bottom: inherit;
  }
  .Hola {
    width: 70%;
  }
  .Hola2 {
    width: 30%;
    display: flex;
    align-items: end;
  }
  .text-class {
    max-width: 80%;
  }
  .display-end {
    display: flex;
    justify-content: end;
  }
}
@media (min-width: 1025px) and (max-width: 1440px) {
  .container {
    display: flex;
    padding-inline: 16px;
  }
  .imagen-class {
    margin-bottom: inherit;
  }
  .Hola {
    width: 80%;
    margin-left: 5rem;
  }
  .Hola2 {
    width: 20%;
    display: flex;
    align-items: end;
  }
  .text-class {
    max-width: 65%;
  }
  .display-end {
    display: flex;
    justify-content: end;
  }
}
@media (min-width: 1441px) {
  .container {
    display: flex;
    padding-inline: 16px;
  }
  .imagen-class {
    margin-bottom: inherit;
  }
  .Hola {
    width: 73%;
    margin-left: 13rem;
  }
  .Hola2 {
    width: 20%;
    display: flex;
    align-items: end;
  }
  .text-class {
    max-width: 61%;

  }
  .display-end {
    display: flex;
    justify-content: end;
  }
}
</style>
