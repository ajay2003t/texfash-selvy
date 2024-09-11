<template>
  <div>
      <div class="contact-container">
        <!-- Left Side: Contact Information -->
        <div class="contact-info">
          <h2>Contact US</h2>
          <div class="info">
            <img src="../assets/address.jpg" class="info">
          </div>
          <div class="social-media">
            <h3>Follow us</h3>
            <div class="social-img">
              <img src="../assets/insta.png" alt="Instagram">
              <img src="../assets/you.png" alt="YouTube">
              <img src="../assets/twitter.png" alt="Twitter">
              <img src="../assets/face.png" alt="Facebook">
            </div>
          </div>
        </div>
    
        <!-- Right Side: Contact Form -->
        <section class="contact-form">
          <div class="form-container">
            <h2 class="form-title">Send a Message</h2>
            <form @submit.prevent="submitForm">
              <div class="name-fields">
                <div class="input-group name-field">
                  <label for="firstName">First Name</label>
                  <input type="text" id="firstName" v-model="firstName" class="input-field" placeholder="First Name" required>
                </div>
                <div class="input-group name-field">
                  <label for="lastName">Last Name</label>
                  <input type="text" id="lastName" v-model="lastName" class="input-field" placeholder="Last Name" required>
                </div>
              </div>
              <div class="input-group">
                <label for="email">Email</label>
                <input type="email" id="email" v-model="email" class="input-field" placeholder="Enter Your Email" required>
              </div>
              <div class="input-group">
                <label for="phone">Phone</label>
                <div class="phone-input">
                  <span class="country-code">+91</span>
                  <input type="tel" id="phone" v-model="phone" class="input-field" placeholder="Enter Phone Number" required>
                </div>
              </div>
              <div class="input-group">
                <label for="message">Message</label>
                <textarea id="message" v-model="message" class="input-field message-area" placeholder="Type Message..." required></textarea>
              </div>
              <button type="submit" class="submit-button">Submit ➔</button>
            </form>
          </div>
        </section>
      </div>
    
    
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style scoped>

.contact-container {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  padding: 40px;
  background-color: white;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  border-radius: 20px;
  width: 80%;
  max-width: 1200px;
  margin: 0 auto;
  margin-top: 4em;
  box-sizing: border-box;
  flex-wrap: wrap;
}

.contact-info {
  flex: 1;
  margin-right: 40px;
  padding: 0em 4em;
  min-width: 250px;
  box-sizing: border-box;
}

.contact-info h2 {
  color: #e07040;
  font-family: "Magra-Bold", Helvetica;
  font-size: 48px;
  font-weight: 700;
  text-align: center;
  margin-bottom: 20px;
}

.info {
  margin-top: 20px;
  font-size: 16px;
  line-height: 1.5;
}

.social-media {
  margin-top: 30px;
}

.social-img {
  display: flex;
  gap: 10px;
  margin-top: 10px;
}

.social-media h3 {
  color: #e07040;
  font-family: "Magra-Bold", Helvetica;
  font-size: 24px;
  font-weight: 700;
  margin-bottom: 10px;
}

.contact-form {
  flex: 1;
  width: 100%;
  max-width: 698px;
  margin: 0 auto;
  display: flex;
  justify-content: center;
  box-sizing: border-box;
  padding: 20px;
}

.form-container {
  background-color: rgba(224, 112, 64, 0.9);
  border-radius: 20px;
  padding: 2em;
  width: 34vw;
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.form-title {
  color: #fff;
  font: 600 32px/1.5 Magra, sans-serif;
  margin-bottom: 20px;
}

.name-fields {
  display: flex;
  justify-content: space-between;
  gap: 20px;
  width: 100%;
}

.name-field {
  flex: 1;
}

.input-group {
  display: flex;
  flex-direction: column;
  width: 100%;
  margin-bottom: 20px;
  margin-left: 2em;
}

.input-group label {
  color: #fff;
  font-size: 15px;
  margin-bottom: 5px;
  font-family: "Poppins-Regular", Helvetica;
}

.input-field {
  width: 90%;
  padding: 12px;
  border: none;
  border-radius: 10px;
  background-color: #fff;
  font-size: 14px;
  color: rgba(0, 0, 0, 0.8);
}

.phone-input {
  display: flex;
  align-items: center;
  background-color: #fff;
  border-radius: 10px;
  padding: 0 10px;
  width: 95%;
  box-sizing: border-box;
}

.country-code {
  color: #000;
  font-size: 14px;
  margin-right: 5px;
}

.message-area {
  width: 90%;
  height: 120px;
  resize: vertical;
}

.submit-button {
  background-color: #fff;
  border: none;
  border-radius: 10px;
  color: rgba(0, 0, 0, 0.8);
  cursor: pointer;
  font-size: 16px;
  font-weight: 400;
  padding: 12px 30px;
  transition: background-color 0.3s ease;
  width: fit-content;
  align-self: center;
  margin-top: 10px;
  margin-left: 11em;
}

.submit-button:hover {
  background-color: #f0f0f0;
}

@media (max-width: 991px) {
  .contact-container {
    flex-direction: column;
    padding: 20px;
  }

  .contact-info, .contact-form {
    width: 100%;
    margin-bottom: 20px;
  }

  .form-container {
    padding: 20px;
  }

  .name-fields {
    flex-direction: column;
  }
}


</style>