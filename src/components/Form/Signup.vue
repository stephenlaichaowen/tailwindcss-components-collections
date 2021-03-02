<template>
  <div class="signup">
    <form>
      <div class="input-username">
        <label>Username</label>
        <input type="text" required placeholder="Username" v-model="username" />
      </div>
      <div class="input-password">
        <label>Password</label>
        <input type="password" required placeholder="**********" v-model="password" />
      </div>
      <div class="input-checkbox">
        <input type="checkbox" />
        <p>Send me your newsletter</p>
      </div>
      <button>Sign up</button>
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
.signup {
  max-width: 520px;
  margin: 0 auto 2rem;
  border: 1px solid #ddd;
  padding: 50px 90px;
}
label {
  font-weight: 700;
  color: #71717a;
  margin-right: 20px;
}
input[type=text],
input[type=password] {
  padding: 8px 12px;
  background: #eee;
  border-radius: 4px;
  width: 225px;
  color: red;
}
.input-username {
  margin-bottom: 24px;
}
.input-password {
  margin-bottom: 22px;
}
.input-checkbox {  
  display: flex;
  align-items: center;
  margin-bottom: 20px;
  margin-left: 90px;
}
.input-checkbox p {
  font-size: 12px;
  color: #71717A;
  font-weight: 700;
}  
input[type=checkbox] {
  margin-right: 8px;
}
button {
  margin-left: 90px;
  padding: 8px 16px;
  background: #A855F7;
  color: white;
  border-radius: 4px;
  font-weight: 500;
}
input[type=checkbox] {
  border-radius: 4px;
}
</style>
