<template>
  <div class="container">
    <h1>Register page</h1>
    <form>
      <div class="form-group row mb-3">
        <label for="email" class="col-sm-2 col-form-label">Email</label>
        <div class="col-sm-8">
          <input
            v-model="email"
            type="email"
            class="form-control"
            id="email"
            aria-describedby="emailHelp"
            required
          />
        </div>
      </div>
      <div class="form-group row mb-3">
        <label for="password" class="col-sm-2 col-form-label">Password</label>
        <div class="col-sm-8">
          <input
            v-model="password"
            type="password"
            class="form-control"
            id="password"
            required
          />
        </div>
      </div>
      <div class="form-group row mb-3">
        <label for="phoneNumber" class="col-sm-2 col-form-label"
          >Phone number</label
        >
        <div class="col-sm-8">
          <input
            v-model="phoneNumber"
            type="number"
            class="form-control"
            id="phoneNumber"
            required
          />
        </div>
      </div>
      <div class="form-group row mb-3">
        <label for="birthday" class="col-sm-2 col-form-label">Birthday</label>
        <div class="col-sm-8">
          <input
            v-model="birthday"
            type="date"
            class="form-control"
            id="birthday"
            required
          />
        </div>
      </div>
      <div class="form-group row mb-3">
        <label for="fullName" class="col-sm-2 col-form-label">Full name</label>
        <div class="col-sm-8">
          <input
            v-model="fullName"
            type="text"
            class="form-control"
            id="fullName"
            required
          />
        </div>
      </div>

      <fieldset class="form-group row mb-4">
        <legend class="col-form-legend col-sm-2">Gender</legend>
        <div class="col-sm-10">
          <div class="form-check">
            <label class="form-check-label">
              <input
                class="form-check-input"
                type="radio"
                name="gridRadios"
                id="gridRadios1"
                value="male"
              />
              Male
            </label>
          </div>
          <div class="form-check">
            <label class="form-check-label">
              <input
                class="form-check-input"
                type="radio"
                name="gridRadios"
                id="gridRadios2"
                value="female"
              />
              Female
            </label>
          </div>
        </div>
      </fieldset>
      <div class="form-group row mb-3">
        <div class="offset-sm-2 col-sm-8">
          <button type="submit" class="btn btn-primary">Register</button>
        </div>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  name: "Login",

  data() {
    return {
      email: "",
      password: "",
      fullName: "",
      phone: "",
      birthday: "",
      gender: "",
    };
  },
};
</script>

<style>
h1 {
  text-align: center;
  margin: 20px 0;
}
form {
  text-align: left;
}
legend {
  font-size: 16px;
}
</style>
