<template>
  <div class="signin">
    <form @submit.prevent="handleSubmit">
      <label>Username</label>
      <input class="username" type="text" placeholder="Username" v-model="username" required />
      <label>Password</label>
      <input
        type="password"
        placeholder="Password"
        v-model="password"
        required
        class="password"
      />
      <small class="warning"><i>Please choose a password</i></small>
      <div class="footer">
        <button>Sign in</button>
        <p class="info">Forget Password?</p>
      </div>
    </form>
  </div>
</template>

<script>
import { ref } from 'vue';

export default {
  setup() {
    const username = ref('')
    const password = ref('')

    const handleSubmit = async () => {
      const info = {
        username: username.value,
        password: password.value
      }
      try {
        // await fetch('')
        console.log(info)
      } catch (error) {
        console.log(error.message)
      }
    }

    return { username, password, handleSubmit }
  }
}
</script>

<style scoped>
.signin {
  max-width: 520px;
  margin: 0 auto 2rem;
  height: 520px;
  background: #e4e4e7;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 100px;
}
form {
  background: #fff;
  padding: 22px 32px 32px 32px;
  border-radius: 4px;
}
label,
input {
  display: block;
}
label {
  margin-bottom: 6px;
  font-weight: 700;
  font-size: 14px;
}
input {
  width: 256px;
  padding: 10px 12px;
  color: #71717A;
  border: 1px solid #ddd;
}
input:focus {
  /* background-color: yellow; */
  border: 1px solid yellow;
}
.username {
  margin-bottom: 14px;
}
.password {
  margin-bottom: 8px;
}
.footer {
  margin-top: 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.info {
  margin-right: 8px;
  font-size: 14px;
  color: #3b82f6;
  font-weight: bold;
}
::placeholder {
  color: #71717A;
  font-size: 16px;
  background: white;
}
button {
  padding: 8px 16px;
  border-radius: 4px;
  background: #3b82f6;
  color: white;
  outline: none;
  transition: all 0.3s ease-in;
}
button:hover {
  /* background-color: #fff;
  color: #3b82f6;
  font-weight: bold; */
  transform: scale(1.1);
}
.warning {
  color: #EF4444;
  font-size: 12px;
}
</style>
