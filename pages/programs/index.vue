<template>
  <div>
    <NavBar />
    <div class="page-container top-container">
      <div class="d-flex flex-column" style="margin-top: 120px">
        <div class="d-flex flex-column align-items-center">
          <div class="heading2" style="color: #c82333; font-size: 28px">
            Programs
          </div>
          <div class="d-flex flex-row" v-for="program in programs">
            <b-card
              :title="program.program_title"
              img-src="https://picsum.photos/600/300/?image=25"
              img-alt="Image"
              img-top
              tag="article"
              style="max-width: 20rem; margin-right: 20px"
              class="mb-2"
            >
              <b-card-text class="description">
                {{ program.description }}
              </b-card-text>
            </b-card>
          </div>
          <div class="subheading2" style="margin-top: 20px">
            Join us in this worthy course
            <b-button
              @click=""
              href="blood-donation"
              style="width: 140px; background-color: #c82333; border: none"
              >Donate</b-button
            >
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
      programs: [
        {
          program_title: "Turkana Feed Programs",
          description:
            "Program initiated on Jan 2022 to feed the hungry at Turkana",
        },
        {
          program_title: "Dadab Attack Response",
          description:
            "In order to get blood donors for the survivors of the Dadab bomb attack, this program was initiated by H.E Kim B",
        },
        {
          program_title: "Turkana Feed Programs",
          description:
            "Program initiated on Jan 2022 to feed the hungry at Turkana",
        },
      ],
    };
  },
};
</script>
