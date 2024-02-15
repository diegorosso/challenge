<template>
  <header class="header" :class="{ active: isNavbarActive }" data-header>
    <div class="container">
      <a href="#" class="logo">
        <img
          src="../assets/Imagenes/Lorem.png"
          width="64"
          height="24"
          alt="Lorem"
        />
      </a>

      <nav class="navbar" :class="{ active: isNavbarActive }" data-navbar>
        <div class="navbar-top">
          <a href="#" class="logo">
            <img
              src="../assets/Imagenes/loremwhite.png"
              width="64"
              height="24"
              alt="Lorem"
            />
          </a>

          <button
            class="nav-close-btn"
            aria-label="close menu"
            data-nav-toggler
            @click="closenav"
          >
            <ion-icon name="close-outline" aria-hidden="true"></ion-icon>
          </button>
        </div>

        <ul class="navbar-list">
          <li>
            <a href="#" class="navbar-link">Home</a>
          </li>

          <li>
            <a href="#" class="navbar-link">About</a>
          </li>

          <li>
            <a href="#" class="navbar-link">Projects</a>
          </li>

          <li>
            <a href="#" class="navbar-link">Blog</a>
          </li>

          <li>
            <a href="#" class="navbar-link">Contact</a>
          </li>
        </ul>

        <div class="wrapper">
          <a href="mailto:info@email.com" class="contact-link"
            >info@email.com</a
          >

          <a href="tel:001234567890" class="contact-link">00 (123) 456 78 90</a>
        </div>

        <ul class="social-list">
          <li>
            <a href="#" class="social-link">
              <ion-icon name="logo-twitter"></ion-icon>
            </a>
          </li>

          <li>
            <a href="#" class="social-link">
              <ion-icon name="logo-facebook"></ion-icon>
            </a>
          </li>


          <li>
            <a href="#" class="social-link">
              <ion-icon name="logo-instagram"></ion-icon>
            </a>
          </li>

          <li>
            <a href="#" class="social-link">
              <ion-icon name="logo-youtube"></ion-icon>
            </a>
          </li>
        </ul>
      </nav>

      <button
        class="nav-open-btn"
        @click="toggleNavbar"
        aria-label="open menu"
        data-nav-toggler
      >
        <ion-icon name="menu-outline" aria-hidden="true"></ion-icon>
      </button>

      <div
        class="overlay"
        :class="{ active: isNavbarActive }"
        data-nav-toggler
        data-overlay
      ></div>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      isNavbarActive: false,
    };
  },
  methods: {
    toggleNavbar() {
      this.isNavbarActive = !this.isNavbarActive;
      document.body.classList.toggle("nav-active");
    },
    closenav() {
      this.isNavbarActive = false;
    },
  },
};
</script>

<style scoped>
.header {
  position: absolute;
  top: 0;
  left: 0;
  background-color: var(--white);
  width: 100%;
  padding-block: 20px;
  box-shadow: var(--shadow-1);
  z-index: 4;
}

.header.active {
  position: fixed;
  animation: slideIn 0.5s ease forwards;
}

@keyframes slideIn {
  0% {
    transform: translateY(-100%);
  }
  100% {
    transform: translateY(0);
  }
}

.header .container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.nav-open-btn {
  font-size: 3.5rem;
  color: var(--gunmetal);
}

.navbar {
  position: fixed;
  top: 0;
  left: -300px;
  background-color: var(--raisin-black);
  color: var(--white);
  max-width: 300px;
  width: 100%;
  height: 100vh;
  padding: 30px;
  padding-block-end: 40px;
  display: flex;
  flex-direction: column;
  gap: 30px;
  z-index: 2;
  visibility: hidden;
  transition: var(--transition-3);
}

.navbar.active {
  visibility: visible;
  transform: translateX(300px);
}

.navbar-top {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.nav-close-btn {
  background-color: var(--white_a8);
  color: var(--white);
  font-size: 2rem;
  padding: 6px;
  border-radius: var(--radius-circle);
  transition: var(--transition-1);
}

.nav-close-btn ion-icon {
  --ionicon-stroke-width: 50px;
}

.nav-close-btn:is(:hover, :focus-visible) {
  background-color: var(--white_a12);
}

.navbar-list {
  margin-block-end: auto;
}

.navbar-link {
  font-weight: var(--fw-700);
  padding-block: 6px;
}

.contact-link {
  transition: var(--transition-1);
}

.contact-link:is(:hover, :focus-visible) {
  color: var(--cinnamon-satin);
}

.overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100vh;
  background-color: var(--raisin-black);
  pointer-events: none;
  opacity: 0;
  transition: var(--transition-1);
}

.overlay.active {
  pointer-events: all;
  opacity: 0.8;
}
@media (min-width: 992px) {
  .nav-open-btn,
  .navbar-top,
  .navbar .wrapper,
  .overlay {
    display: none;
  }

  .navbar,
  .navbar.active {
    all: unset;
    display: flex;
    flex-grow: 1;
  }

  .navbar-list {
    display: flex;
    gap: 36px;
    margin-inline: auto;
  }

  .navbar-link {
    color: var(--charcoal);
    transition: var(--transition-1);
  }

  .navbar-link:is(:hover, :focus-visible) {
    color: var(--cinnamon-satin);
  }

  .navbar .social-link {
    color: var(--charcoal);
    font-size: 1.8rem;
  }

  .header {
    left: 50%;
    transform: translateX(-50%);
    padding-inline: 16px;
    border-radius: var(--radius-8);
  }

  .header.active {
    top: 0;
    left: 0;
    max-width: unset;
    border-radius: 0;
  }
}

</style>
