<template>
  <b-row class="vh-100 vw-100 row-login">
    <b-col class="d-flex justify-content-center align-items-center center-login">
      <div class="col-8">
        <b-form class="formul">
          <b-form-group
            label="E-mail"
            label-for="email"
            >
              <b-form-input
                id="email"
                type="email"
                autocomplete="off"
                v-model="form.email"
              ></b-form-input>
            </b-form-group>
 
            <b-form-group
              label-for="password"
            >
              <label class="d-flex justify-content-between">
                Senha
              </label>
 
              <b-form-input
                id="password"
                type="password"
                v-model="form.password"
              ></b-form-input>
            </b-form-group>
            <br>
            <br>
            <b-button
              id="button"
              type="button"
              block>
              <i class="fas fa-sign-in-alt"></i> Login
            </b-button>
 
        </b-form>
      </div>
    </b-col>
  </b-row>
</template>
 
<script>
 
export default {
  data() {
    return {
      form: {
        email: "",
        password: ""
      }
    }
  },
 
  methods: {
    login() {},
 
  }
}
</script>
 
<style>
 
*, /*resetar o estilo da página*/
*::after,
*::before {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
}
 
.row-login {
  margin-left: 0;
}

.formul{
 align-items: center;
 justify-content: center;
}
 
.center-login {
  background-color: #F2F2F2;
}

#email.form-control {
  background-color: #C4C4C4;
  padding: 2vh;
}
#password.form-control {
  background-color: #C4C4C4;
  padding: 2vh;
}

#button{
  background-color: #757575;
  padding: 1vh;
}


 
</style>