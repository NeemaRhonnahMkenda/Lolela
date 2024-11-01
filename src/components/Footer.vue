<template>
  <div class="lolela-footer mt-10">
    <div class="footer-content">
      <p class="footer-heading">LOLELA.</p>

      <div class="footer-links">
        <div class="contact-info">
          <i class="fa fa-envelope" aria-hidden="true" style="font-size: 24px; color: white;"></i>
          <p class="email-text">lolela-zm@gmail.com</p>
        </div>

        <div class="policy-links">
          <p class="policy-text">Privacy Policy</p>
          <p class="policy-text">Terms and Conditions</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AppFooter',
  data() {
    return {}
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Bellota:ital,wght@0,300;0,400;0,700;1,300;1,400;1,700&display=swap');

.lolela-footer {
  background-color: #A47556;
  padding-top: 30px;
}

.footer-content {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  margin-left: 80px;
}

.footer-heading {
  font-size: 50px;
  color: #A47556;
  background-color: #E3CDC1;
  width: fit-content;
  margin-top: 20px;
}

.contact-info {
  display: flex;
  align-items: center;
  color: white;
  margin-top: 20px;
}

.email-text {
  font-size: 15px;
  font-family: Bellota, cursive;
  margin-left: 10px;
}

.footer-links {
  display: flex;
  justify-content: space-between;
  width: 100%;
  margin-top: 150px;
  margin-bottom: 40px;
}

.policy-links {
  display: flex;
  align-items: center;
  color: white;
  margin-right: 80px;
}

.policy-text {
  font-size: 15px;
  font-family: Bellota, cursive;
  margin-left: 20px;
}
</style>
