<template lang="en">
  <div>
    <form class="d-grid w-50 mx-auto gap-2">
        <label for="fullname">Fullname</label>
        <input type="text" placeholder="Fullname..." v-model="fullname">
        <label for="email">Email</label>
        <input type="email" placeholder="Email..." v-model="email">
        <label for="age">Age</label>
        <input type="number" placeholder="Age..." v-model="age">
        <label for="dob">DOB</label>
        <input type="date" placeholder="DOB..." v-model="dob">
        <input type="submit" class="w-25 mx-auto mb-5" id="submit" placeholder="Submit" v-on:click.prevent="submit">
    </form> 
  </div>
</template>
<script>
export default {
  methods: {
    submit() {
      alert(`${this.fullname} with the email ${this.email} at age ${this.age} was born on ${this.dob}`)
    }
  },
}
</script>

<style scoped>

</style>


<!-- <template>
  <div class="contact">
    <h1>Send us a message:</h1>
  </div>

  <form>

    <div class="form-outline mb-4 w-50 mx-auto">
      <input type="text" id="form4Example1" class="form-control" placeholder="Enter Name" />
    </div>


    <div class="form-outline mb-4 w-50 mx-auto">
      <input type="email" id="form4Example2" class="form-control" placeholder="Enter Email" />
    </div>

    <div class="form-outline mb-4 w-50 mx-auto">
      <textarea class="form-control" placeholder="Enter Message" id="form4Example3" rows="4"></textarea>

    </div>


    <div class="form-check d-flex justify-content-center mb-4 w-50 mx-auto">
      <input class="form-check-input me-2" placeholder="Enter" type="checkbox" value="" id="form4Example4" checked />
      <label class="form-check-label" for="form4Example4">
        Send me a copy of this message
      </label>
    </div>

    <button type="submit" class="btn btn-light btn-block mb-4">Send</button>
  </form>

</template>

<style scoped>
</style> -->


  