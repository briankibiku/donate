<template>
  <div>
    <NavBar />
    <div class="page-container top-container" >
      <div class="d-flex flex-column" style="margin-top: 20vh">
        <div class="d-flex flex-column align-items-center">
          <img
            src="~assets/images/phone-call.png"
            alt=""
            height="120"
            width="120"
            style="margin-right: 20px"
          />
          <div class="heading2" style="color: #c82333; font-size: 28px">
            Contact US
          </div>

          <div class="heading2">Get in touch...</div>
          <div class="d-flex flex-row">
            <div class="col">
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
                    type="textarea"
                    placeholder="Message"
                    v-model="message"
                    required
                    style="margin-bottom: 10px"
                  />
                </div>
              </form>
              <b-button @click="" class="primary-button" style="width: 100%"
                >Send</b-button
              >
            </div>
          </div>
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
      message: "",
      blood_type: "",
    };
  },
};
</script>
