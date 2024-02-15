<template>
  <section class="section hero" aria-label="home">
    <div class="container">
      <figure class="hero-banner">
        <img
          src="../assets/Imagenes/dna.jpg"
          width="560"
          height="540"
          alt="Julia"
          class="w-100"
          data-reveal="top"
        />
      </figure>

      <div class="hero-content">
        <h1 class="h1 hero-title" data-reveal="top" data-reveal-delay="0.5s">
          Lorem ipsum dolor sit amet consectetur.
        </h1>

        <p class="section-text" data-reveal="top" data-reveal-delay="0.75s">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Asperiores
          culpa veniam natus adipisci excepturi sapiente! Repellat maiores
          minima deserunt placeat modi ullam?
        </p>

        <div class="btn-wrapper" data-reveal="top" data-reveal-delay="1s">
          <a href="#" class="btn btn-secondary">Lorem, ipsum.</a>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.hero {
  padding-block-start: calc(var(--section-padding) + 50px);
  background-color: var(--cultured);
}

.hero .container {
  display: grid;
  gap: 50px;
}

.hero-banner {
  position: relative;
  max-width: max-content;
  margin-inline: auto;
}

.hero-content {
  text-align: center;
}

.hero .section-text {
  margin-block: 24px 36px;
}

.hero-content {
  text-align: center;
}
.hero .section-text {
  margin-block: 24px 36px;
}
.btn-wrapper {
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 12px;
}
@media (min-width: 992px) {
  .hero {
    padding-block-start: calc(var(--section-padding) + 80px);
  }

  .hero .container {
    grid-template-columns: 0.8fr 1fr;
    align-items: center;
    gap: 100px;
  }

  .hero-content {
    text-align: left;
  }

  .hero .btn-wrapper {
    justify-content: flex-start;
  }
}

@media (min-width: 1400px) {
  .hero .container {
    grid-template-columns: 1fr 0.8fr;
  }

  .hero .section-text {
    --fs-5: 2.4rem;
  }
}
</style>
