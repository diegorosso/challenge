<template>
  <section class="container">
    <!-- div1 -->
    <div class="mediaquery-one">
      <div class="background">
        <h1 class="title">Internal Line</h1>
        <div class="container-width">
          <p class="class-style">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sit,
            minus. Sed praesentium maiores laudantium eos cum explicabo ad
            dolorum sunt!
          </p>
        </div>
        <div class="container-icon">
          <ion-icon class="icon-style" name="arrow-forward-outline"></ion-icon>
        </div>
      </div>
      <!-- div2 -->
      <div class="background-2">
        <h1 class="title">Internal Line</h1>
        <div class="container-width">
          <p class="class-style">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sit,
            minus. Sed praesentium maiores laudantium eos cum explicabo ad
            dolorum sunt!
          </p>
        </div>
        <div class="container-icon">
          <ion-icon class="icon-style" name="arrow-forward-outline"></ion-icon>
        </div>
      </div>
    </div>
    <!-- div3 -->
    <div class="mediaquery-two">
      <div class="background-3">
        <h1 class="title">Internal Line</h1>
        <div class="container-width">
          <p class="class-style">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sit,
            minus. Sed praesentium maiores laudantium eos cum explicabo ad
            dolorum sunt!
          </p>
        </div>
        <div class="container-icon">
          <ion-icon class="icon-style" name="arrow-forward-outline"></ion-icon>
        </div>
      </div>
      <!-- div4 -->
      <div class="background-4">
        <h1 class="title">Internal Line</h1>
        <div class="container-width">
          <p class="class-style">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sit,
            minus. Sed praesentium maiores laudantium eos cum explicabo ad
            dolorum sunt!
          </p>
        </div>
        <div class="container-icon">
          <ion-icon class="icon-style" name="arrow-forward-outline"></ion-icon>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.container {
  width: 100%;
}
.container-width {
  max-width: 90%;
}
.background {
  background-color: #7d9ac2;
  padding: 10px;
  margin-bottom: 2rem;
}
.title {
  font-size: var(--fs-1);
  color: var(--white);
}
.class-style {
  color: var(--raisin-black);
}

.container-icon {
  width: 95%;
  display: flex;
  justify-content: end;
  cursor: pointer;
}
.icon-style {
  border: solid 1px var(--raisin-black);
  padding: 1rem;
  font-size: 2rem;
  color: var(--raisin-black);
}
.background-2 {
  background-color: #a4b9d4;
  padding: 10px;
  margin-bottom: 2rem;
}
.background-3 {
  background-color: #d8e2ee;
  padding: 10px;
  margin-bottom: 2rem;
}
.background-4 {
  background-color: #b8c8df;
  padding: 10px;
  margin-bottom: 2rem;
}
@media (max-width: 600px) {
  .container {
    flex-direction: column;
  }
  .mediaquery-one {
    flex-direction: column;
  }
  .mediaquery-two {
    flex-direction: column;
  }
  .class-style {
    width: 85%;
  }
  .background {
    margin-bottom: inherit;
  }
  .background-2 {
    margin-bottom: inherit;
  }
  .background-3 {
    margin-bottom: inherit;
  }
}

@media (min-width: 601px) and (max-width: 1024px) {
  .mediaquery-one {
    display: flex;
  }
  .mediaquery-two {
    display: flex;
  }
  .background {
    margin-bottom: inherit;
  }
  .background-2 {
    margin-bottom: inherit;
  }
  .background-3 {
    margin-bottom: inherit;
  }
  .background-4 {
    margin-bottom: inherit;
  }
}
@media (min-width: 1025px) and (max-width: 1440px) {
  .container {
    display: flex;
  }
  .mediaquery-one {
    display: flex;
  }
  .mediaquery-two {
    display: flex;
  }
}
@media (min-width: 1441px) {
  .container {
    display: flex;
  }
  .mediaquery-one {
    display: flex;
  }
  .mediaquery-two {
    display: flex;
  }
}

</style>
