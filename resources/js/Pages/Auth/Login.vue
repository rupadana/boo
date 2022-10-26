<template>
  <div>
    <div id="auth">
      <div class="row h-100">
        <div class="col-lg-5 col-12">
          <div id="auth-left">
            <div class="auth-logo">
              <a href="#"
                ><img src="/vendor/mazer/assets/images/logo/logo.svg" alt="Logo"
              /></a>
            </div>
            <h1 class="auth-title">Log in.</h1>
            <p class="auth-subtitle mb-5">
              Log in with your data that you entered during registration.
            </p>

            <form action="#" @submit.prevent="submit">
              <div class="form-group position-relative has-icon-left mb-4">
                <input
                  type="text"
                  class="form-control form-control-xl"
                  :class="{
                    'is-invalid' : form.errors.email
                  }"
                  placeholder="Email"
                  v-model="form.email"
                />
                <div class="form-control-icon">
                  <i class="bi bi-person"></i>
                </div>
                <div class="invalid-feedback" style="display:block" v-if="form.errors.email">
                  <i class="bx bx-radio-circle"></i>
                  {{form.errors.email}}
                </div>
              </div>
              <div class="form-group position-relative has-icon-left mb-4">
                <input
                  v-model="form.password"
                  type="password"
                  class="form-control form-control-xl"
                  placeholder="Password"
                  :class="{
                    'is-invalid' : form.errors.password
                  }"
                />
                <div class="form-control-icon">
                  <i class="bi bi-shield-lock"></i>
                </div>
                <div class="invalid-feedback" style="display:block" v-if="form.errors.password">
                  <i class="bx bx-radio-circle"></i>
                  {{form.errors.password}}
                </div>
              </div>
              <div class="form-check form-check-lg d-flex align-items-end">
                <input
                  class="form-check-input me-2"
                  type="checkbox"
                  value=""
                  id="flexCheckDefault"
                />
                <label
                  class="form-check-label text-gray-600"
                  for="flexCheckDefault"
                >
                  Keep me logged in
                </label>
              </div>
              <button class="btn btn-primary btn-block btn-lg shadow-lg mt-5">
                Log in
              </button>
            </form>
            <div class="text-center mt-5 text-lg fs-4">
              <p class="text-gray-600">
                Don't have an account?
                <a href="auth-register.html" class="font-bold">Sign up</a>.
              </p>
              <p>
                <a class="font-bold" href="auth-forgot-password.html"
                  >Forgot password?</a
                >.
              </p>
            </div>
          </div>
        </div>
        <div class="col-lg-7 d-none d-lg-block">
          <div id="auth-right"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    name:String,
  },
  methods: {
    submit() {
      this.form.post("/login");
    },
  },
  data() {
    return {
      form: this.$inertia.form({
        email: "",
        password: "",
        remember: false,
      }),
    };
  },
};
</script>

<style>
</style>