<template>
  <div>
    <NavBar />
    <div class="page-container top-container" >
      <div class="d-flex flex-column" style="margin-top: 20vh">
        <div class="d-flex flex-column align-items-center">
          <img
            src="~assets/images/donate_pint.png"
            alt=""
            height="120"
            width="120"
            style="margin-right: 20px"
          />
          <div class="heading2" style="color: #c82333; font-size: 28px">
            Donate Blood
          </div>

          <div class="heading2">Let's start by knowing you...</div>
          <form action="">
            <div class="form-group d-flex flex-column justify-content-left">
              <input
                class="border-input"
                type="text"
                placeholder="User Name"
                v-model="donor_name"
                required
                style="margin-bottom: 10px"
              />
              <input
                class="border-input"
                type="number"
                placeholder="Phone Number"
                v-model="phone_number"
                required
                style="margin-bottom: 10px"
              />
              <b-form-select
                id="inline-form-custom-select-pref"
                class="mb-2 mr-sm-2 mb-sm-0"
                :options="[
                  { text: 'Blood type...', value: null },
                  'A+',
                  'A-',
                  'B+',
                  'B-',
                  'O+',
                  'O-',
                  'AB+',
                  'AB-',
                ]"
                :value="null"
              ></b-form-select>
            </div>
          </form>
          <b-button @click="" class="primary-button">Sign Up</b-button>
          <div class="subheading2">
            Did you know that your blood can save upto <b> four </b> lives?
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      donor_name: "",
      phone_number: "",
      blood_type: "",
    };
  },
};
</script>
