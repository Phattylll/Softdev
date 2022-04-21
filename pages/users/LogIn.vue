<template lang="html">
<div class="center">
    <v-text-field v-model="email" label="Email"></v-text-field>
    <v-text-field
      v-model="password"
      label="Password"
      type="password"
    ></v-text-field>
    <!-- <v-btn  @click="handleLoginClicked"> Login</v-btn> -->
 


</style>

<button type="button" class="cancelbtn">Cancel</button>



  </div>

</template>


<script>
export default {
  layout: 'session',
  data() {
    return {
      email: '',
      password: ''
    }
  },
  methods: {
    async handleLoginClicked() {
      try {
        const response = await this.$auth.loginWith('local', {
          data: { user: { email: this.email, password: this.password } }
        })
        console.log(response)
        if (response.data.success) {
          this.$router.replace({ name: 'blogs' })
        }
      } catch (err) {
        console.log(err)
      }
    }
  }
}
</script>

<style lang="css" scoped></style>



<style>
.center {
  margin: 100px auto;
  width: 60%;
  border: 4px solid rgb(243, 95, 16);
  padding: 30px;
  padding-top: 10px;
  padding-bottom: 150px;

}

  .cancelbtn {
      float: right;
      margin: 90px 0 12px 0;
      width: auto;
      padding: 7px 15px;
      background-color: #f44336;
    }

</style>



<script>
export default {
    layout:"Hbar"
}
</script>

