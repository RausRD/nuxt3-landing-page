<template>
  <div class="feedback-form-wrapper">
    <h2>Send your data</h2>
    <form class="feedback-form">
      <input v-model="firstName" type="text" placeholder="First Name" />
      <input v-model="secondName" type="text" placeholder="Second Name" />
      <input v-model="email" type="email" placeholder="Email" />
      <input v-model="address" type="text" placeholder="Address" />
      <input type="submit" class="form-submit" @click="onFormSubmit" />
    </form>
  </div>
</template>

<script setup>
const firstName = useState('firstName')
const secondName = useState('secondName')
const email = useState('email')
const address = useState('address')

const onFormSubmit = (event) => {
  event.preventDefault()
  console.log(`  First Name: ${firstName.value}
  Second Name: ${secondName.value}
  Email: ${email.value}
  Address: ${address.value}`)
}
</script>

<style scoped>
.feedback-form-wrapper {
  height: 560px;
  background-image: url(~/assets/svg/waves-background.svg);
  background-repeat: no-repeat;
  background-size: cover;
  text-align: center;
  padding: 60px 420px;
  border-bottom-right-radius: 30px;
  border-top-right-radius: 30px;
}

h2 {
  color: #fff;
  margin-bottom: 17px;
}

.feedback-form {
  display: flex;
  flex-direction: column;
}

.feedback-form input {
  width: 392px;
  height: 58px;
  font-size: 18px;
  line-height: 28px;
  padding: 15px 30px;
  margin-bottom: 16px;
  border-radius: 38px;
  border: 1px solid #c8c2c6;
  background-color: #fff;
}

.feedback-form input::placeholder {
  color: var(--text-color-placeholder);
}

.feedback-form .form-submit {
  background-color: var(--color-accent);
  border: none;
  color: #fff;
  cursor: pointer;
}
</style>
