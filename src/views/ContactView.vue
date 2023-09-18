<template>
  <div class="container text-center">
    <div class="row align-items-start" id="cont">
      <h1>Connect with me Here</h1>
      <div class="col-md-6">
        <form action="https://formspree.io/f/xjvqvbdn" method="post" ref="myForm" @submit.prevent="handleSubmit">
          <div class="mb-3">
            <label for="exampleFormControlInput1" class="form-label">First name</label>
            <input type="text" class="form-control" name="name" id="exampleFormControlInput1" v-model="firstName"
              :class="{ 'is-invalid': formSubmitted && !firstName }"
              :placeholder="getPlaceholder('Please enter your name', formSubmitted && !firstName)">
            <div v-if="formSubmitted && !firstName" class="invalid-feedback">Please enter your name</div>
          </div>
          <div class="mb-3">
            <label for="exampleFormControlInput2" class="form-label">Last name</label>
            <input type="text" class="form-control" name="name" id="exampleFormControlInput2" v-model="lastName"
              :class="{ 'is-invalid': formSubmitted && !lastName }"
              :placeholder="getPlaceholder('Please enter your surname', formSubmitted && !lastName)">
            <div v-if="formSubmitted && !lastName" class="invalid-feedback">Please enter your surname</div>
          </div>
          <div class="mb-3">
            <label for="exampleFormControlInput3" class="form-label">Email address</label>
            <input type="email" class="form-control" name="name" id="exampleFormControlInput3" v-model="email"
              :class="{ 'is-invalid': formSubmitted && !email }"
              :placeholder="getPlaceholder('Please enter your email', formSubmitted && !email)">
            <div v-if="formSubmitted && !email" class="invalid-feedback">Please enter your email</div>
          </div>
          <div class="mb-3">
            <label for="exampleFormControlTextarea1" class="form-label">Write your message</label>
            <textarea class="form-control" id="exampleFormControlTextarea1" rows="6" v-model="textareaContent"
              :class="{ 'is-invalid': formSubmitted && !textareaContent }"
              :placeholder="getPlaceholder('Please enter your message', formSubmitted && !textareaContent)"></textarea>
            <div v-if="formSubmitted && !textareaContent" class="invalid-feedback">Please enter your message</div>
          </div>
          <div class="btn d-flex">
            <button type="submit">Submit</button>
            <button type="button" @click="clearForm">Clear Form</button>
          </div>
        </form>
      </div>
      <div class="col-md-6">
        <div class="col-12 iframe-container">
          <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d13232.179982065223!2d18.68425895!3d-33.991378000000005!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x1dcc4ef22e100303%3A0x9c679ad8b97c4b16!2sFountain%20Village%2C%20Cape%20Town%2C%207100!5e0!3m2!1sen!2sza!4v1695051609078!5m2!1sen!2sza" width="600" height="300" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>
        <p>call me:0634854531</p>
        <p>email: zwenisiyamanga@gmail.com</p>
        <div class="social-icons">
          <a href="https://www.linkedin.com/in/siyamanga-zweni-20099b1aa/" target="_blank" rel="noopener noreferrer">
            <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" fill="currentColor" class="bi bi-linkedin"
              viewBox="0 0 16 16">
              <path
                d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854V1.146zm4.943 12.248V6.169H2.542v7.225h2.401zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248-.822 0-1.359.54-1.359 1.248 0 .694.521 1.248 1.327 1.248h.016zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016a5.54 5.54 0 0 1 .016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225h2.4z" />
            </svg>
          </a>
          <a href="https://github.com/" target="_blank" rel="noopener noreferrer">
            <svg class="bi bi-github" width="30" height="30" fill="currentColor" viewBox="0 0 16 16">
              <path
                d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.49-.94-.84-1.13-.29-.14-.71-.49-.01-.5.66-.01 1.13.61 1.28.87.75 1.26 1.95.9 2.43.68.07-.52.29-.9.53-1.11-1.86-.21-3.82-.93-3.82-4.13 0-.91.32-1.65.85-2.23-.09-.21-.37-1.05.08-2.19 0 0 .69-.22 2.27.85.66-.18 1.37-.27 2.08-.27s1.42.09 2.08.27c1.58-1.07 2.27-.85 2.27-.85.45 1.14.17 1.98.08 2.19.53.58.85 1.32.85 2.23 0 3.2-1.96 3.92-3.83 4.13.3.26.57.77.57 1.56 0 1.13-.01 2.04-.01 2.31 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z" />
            </svg>
          </a>
          <a href="//wa.me/0634854531" target="_blank" rel="noopener noreferrer">
            <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" fill="currentColor" class="bi bi-whatsapp" viewBox="0 0 16 16">
              <path d="M13.601 2.326A7.854 7.854 0 0 0 7.994 0C3.627 0 .068 3.558.064 7.926c0 1.399.366 2.76 1.057 3.965L0 16l4.204-1.102a7.933 7.933 0 0 0 3.79.965h.004c4.368 0 7.926-3.558 7.93-7.93A7.898 7.898 0 0 0 13.6 2.326zM7.994 14.521a6.573 6.573 0 0 1-3.356-.92l-.24-.144-2.494.654.666-2.433-.156-.251a6.56 6.56 0 0 1-1.007-3.505c0-3.626 2.957-6.584 6.591-6.584a6.56 6.56 0 0 1 4.66 1.931 6.557 6.557 0 0 1 1.928 4.66c-.004 3.639-2.961 6.592-6.592 6.592zm3.615-4.934c-.197-.099-1.17-.578-1.353-.646-.182-.065-.315-.099-.445.099-.133.197-.513.646-.627.775-.114.133-.232.148-.43.05-.197-.1-.836-.308-1.592-.985-.59-.525-.985-1.175-1.103-1.372-.114-.198-.011-.304.088-.403.087-.088.197-.232.296-.346.1-.114.133-.198.198-.33.065-.134.034-.248-.015-.347-.05-.099-.445-1.076-.612-1.47-.16-.389-.323-.335-.445-.34-.114-.007-.247-.007-.38-.007a.729.729 0 0 0-.529.247c-.182.198-.691.677-.691 1.654 0 .977.71 1.916.81 2.049.098.133 1.394 2.132 3.383 2.992.47.205.84.326 1.129.418.475.152.904.129 1.246.08.38-.058 1.171-.48 1.338-.943.164-.464.164-.86.114-.943-.049-.084-.182-.133-.38-.232z"/>
            </svg>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      firstName: '',
      lastName: '',
      email: '',
      textareaContent: '',
      formSubmitted: false,
    };
  },
  methods: {
    clearForm() {
      this.firstName = '';
      this.lastName = '';
      this.email = '';
      this.textareaContent = '';
      this.formSubmitted = false;
      this.$refs.myForm.reset();
    },
    handleSubmit() {
      this.formSubmitted = true;

      if (!this.firstName || !this.lastName || !this.email || !this.textareaContent) {
        return;
      }

      this.$refs.myForm.submit();
    },
    getPlaceholder(defaultPlaceholder, isInvalid) {
      if (isInvalid) {
        return 'Please fill in the required field';
      } else {
        return defaultPlaceholder;
      }
    },
  },
};
</script>
<style>
.container {
  display: flex;
  align-items: center;
  justify-content: center;
}

#cont {
  background-color: rgba(222,227,229,255);

  border-radius: 8px;
}

.is-invalid {
  border-color: red !important;
}

.is-invalid::placeholder {
  color: red !important;
}

.btn {
  justify-content: space-between;
  padding: 8px;
  border-radius: 10px;
}

button {
  border: 1px solid#999fa0;
  padding: 2px;
  background-color: #999fa0;
  color: black;
  border-radius: 12px;
  box-shadow: 5px 10px 0px black;
}

.social-icons {
  display: flex;
  justify-content: center;
  margin-bottom: 1rem;
  animation: pulse;
  animation-duration: 2s;
  animation-iteration-count: infinite;
}

.social-icons a {
  display: inline-block;
  margin: 0 0.5rem;
  color: #000;
  transition: color 0.3s ease;
}
@media(width<770px){
  .container{
    margin-top: 20px;
    margin-bottom: 40px;
    
  }
}
</style>