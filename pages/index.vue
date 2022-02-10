<template>
  <div>
    <NavBar />
    <div class="page-container centered-container">
      <div class="d-flex flex-column align-items-center">
        <div class="heading1">Donate to save a life</div>
        <div class="d-flex flex-row align-items-center">
          <div class="heading2">I wish to donate</div>
        </div>
        <div>
          <b-button
            @click=""
            href="/blood-donation"
            style="width: 160px; background-color: #c82333; border: none"
            >Blood</b-button
          >
          <b-button
            @click=""
            href="/money-donation"
            style="width: 160px; background-color: #c82333; border: none"
            >Money</b-button
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
@media only screen and (max-width: 600px) {
  .heading1 {
    font-size: 40px;
    font-weight: 900;
    padding-bottom: 10px;
    color: rgb(121, 117, 117);
    font-family: "Nunito Sans", sans-serif;
  }
}
</style>
