<template>
  <div class="row d-flex justify-content-center">
    <div class="col-lg-6 col-md-8 col-sm-12">
        <form @submit.prevent="handleSubmit()">
        <div class="container">
          <div class="heading">SignIn to your account</div>
          <div class="input-field">
            <input
              type="text"
              class="form-control"
              id="memEmail"
              autocomplete="off"
              required
              placeholder="Email"
              v-model.trim="memEmail"
            />
            <label for="memEmail">Email</label>
          </div>
          <div class="input-field">
            <input
              type="text"
              class="form-control"
              id="memName"
              autocomplete="off"
              required
              placeholder="Name"
              v-model.trim="memName"
            />
            <label for="memName">Name</label>
          </div>
          <div class="input-field">
              <input
                type="password"
                class="form-control"
                id="password"
                autocomplete="off"
                required
                placeholder="Password"
                v-model.trim="password"
              />
              <label for="password">Password</label>
          </div>
          <div class="btn-container">
            <button class="btn" type="submit">ตกลง</button>
          </div>
        </div>
      </form>
      <!-- ส่วนแสดงสถานะ จากการตอบกลับของ Backend -->
      <p v-if="backendMessage == 'success'" class="alert alert-success mt-3">
        ลงทะเบียนสำเร็จ-{{ backendMessage }}
      </p>
      <p v-else-if="backendMessage == 'fail'" class="alert alert-danger mt-3">
        ลงทะเบียนผิดพลาด-{{ backendMessage }}
      </p>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  name: "TheRegister",
  data() {
    return {
      memEmail: null,
      memName: null,
      password: null,
      backendMessage: null,
    };
  },
  methods: {
    async handleSubmit() {
      let members = {
        memEmail: this.memEmail,
        memName: this.memName,
        password: this.password,
      };
      try {
        const response = await axios.post(
          `http://localhost:3000/members`,
          members
        );
        this.backendMessage = response.data.messageregister;
      } catch (err) {
        console.log(err);
      }
    },
  },
};
</script>

<style scoped>
.card {
  background-color: #fffdfd;
}

.card-body {
  padding: 2rem;
}

.card-title {
  font-size: 1.5rem;
  font-weight: 500;
}

.form-floating > input::placeholder {
  color: #6c757d;
}

.btn-primary {
  background-color: #007bff;
  border: none;
}

.btn-primary:hover {
  background-color: #0056b3;
}

.alert {
  font-size: 0.875rem;
}

/* From Uiverse.io by Spacious74 */ 
.container {
  border: solid 1px #8d8d8d;
  padding: 20px;
  border-radius: 20px;
  background-color: #fff;
}

.container .heading {
  font-size: 1.3rem;
  margin-bottom: 20px;
  font-weight: bolder;
}

.form {
  max-width: 300px;
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.form .btn-container {
  width: 100%;
  display: flex;
  align-items: center;
  gap: 20px;
}

.form .btn {
  padding: 10px 20px;
  font-size: 1rem;
  text-transform: uppercase;
  letter-spacing: 3px;
  border-radius: 10px;
  border: solid 1px #1034aa;
  border-bottom: solid 1px #90c2ff;
  background: linear-gradient(135deg, #0034de, #006eff);
  color: #fff;
  font-weight: bolder;
  transition: all 0.2s ease;
  box-shadow: 0px 2px 3px #000d3848, inset 0px 4px 5px #0070f0,
    inset 0px -4px 5px #002cbb;
}

.form .btn:active {
  box-shadow: inset 0px 4px 5px #0070f0, inset 0px -4px 5px #002cbb;
  transform: scale(0.995);
}

.input-field {
  position: relative;
}

.input-field label {
  position: absolute;
  color: #8d8d8d;
  pointer-events: none;
  background-color: transparent;
  left: 15px;
  transform: translateY(0.6rem);
  transition: all 0.3s ease;
}

.input-field input {
  padding: 10px 15px;
  font-size: 1rem;
  border-radius: 8px;
  border: solid 1px #8d8d8d;
  letter-spacing: 1px;
  width: 100%;
}

.input-field input:focus,
.input-field input:valid {
  outline: none;
  border: solid 1px #0034de;
}

.input-field input:focus ~ label,
.input-field input:valid ~ label {
  transform: translateY(-51%) translateX(-10px) scale(0.8);
  background-color: #fff;
  padding: 0px 5px;
  color: #0034de;
  font-weight: bold;
  letter-spacing: 1px;
  border: none;
  border-radius: 100px;
}

.form .passicon {
  cursor: pointer;
  font-size: 1.3rem;
  position: absolute;
  top: 6px;
  right: 8px;
}

.form .close {
  display: none;
}

</style>