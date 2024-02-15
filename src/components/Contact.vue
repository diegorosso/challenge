<template>
  <div class="container-contact">
    <h1 class="contact-align">Contacto</h1>
    <div class="contact-info">
      <div class="contact-item">
        <ion-icon name="location-outline"></ion-icon>
        <p>Dirección: 123 Calle Principal, Ciudad, País</p>
      </div>
      <div class="contact-item">
        <ion-icon name="mail-outline"></ion-icon>
        <p>Email: ejemplo@correo.com</p>
      </div>
      <div class="contact-item">
        <ion-icon name="call-outline"></ion-icon>
        <p>Teléfono: +123 456 789</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container-contact {
  background-color: var(--charcoal);;
  padding: 30px;
  color: white;
}

.contact-info {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: column;
}

.contact-item {
  display: flex;
  align-items: center;
}

.contact-item ion-icon {
  font-size: 24px;
  margin-right: 10px;
}
.contact-align{
    text-align: center;
}
</style>
