<template>
  <div class="contact container">
    <div class="text-center">
      <h1 class="display-4">Contact Us</h1>
      <h5>
        555-555-5555 <br />
        5515 Main St - Lawton, OK
      </h5>
    </div>
    <br /><br />
    <form>
      <!-- Name input -->
      <div class="form-outline mb-4">
        <input type="text" id="form4Example1" class="form-control" />
        <label class="form-label" for="form4Example1">Name</label>
      </div>
      <!-- Email input -->
      <div class="form-outline mb-4">
        <input type="email" id="form4Example2" class="form-control" />
        <label class="form-label" for="form4Example2">Email address</label>
      </div>
      <!-- file upload -->
      <label class="form-label" for="customFile">File Upload</label>
      <input type="file" class="form-control" id="customFile" />
      <br />
      <!-- Message input -->
      <div class="form-outline mb-4">
        <textarea class="form-control" id="form4Example3" rows="4"></textarea>
        <label class="form-label" for="form4Example3">Message</label>
      </div>
      <!-- Checkbox -->
      <div class="form-check d-flex justify-content-center mb-4">
        <input
          class="form-check-input me-2"
          type="checkbox"
          value=""
          id="form4Example4"
          checked
        />
        <label class="form-check-label" for="form4Example4">
          Send me a copy of this message
        </label>
      </div>
      <!-- Submit button -->
      <button type="submit" class="btn btn-primary btn-block mb-4">Send</button>
    </form>
  </div>
</template>

<script></script>

<style lang="scss">
//code here
.contact {
  margin-top: 60px;
  form {
    max-width: 750px;
    margin-left: auto;
    margin-right: auto;
  }
  input {
    background-color: rgb(228, 222, 222) !important;
  }
  textarea {
    background-color: rgb(228, 222, 222) !important;
  }
}
</style>
