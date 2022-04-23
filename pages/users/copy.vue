<template lang="html">
<div class="center">
  <nuxt-link button type="button"  class="cancelbtn" to ="/users/Newpass"><h3 style="color:white">NEXT</h3></button></button></nuxt-link>
  <!-- <button type="button"  class="cancelbtn" to ="/users/Newpass"><h3 style="color:white">NEXT</h3></button></button> -->
    <v-text-field v-model="email" label="Email"></v-text-field>
    
    <!-- <v-btn  @click="handleLoginClicked"> Login</v-btn> -->
 


</style>
<div class="box Hw"><h1 style="color:rgb(243, 95, 16)">Reset Password</h1></div>
  </div>
</template>

 
<script>
export default {
   layout:"Hbar",
  data() {
    return {
      email: '',
      password: '',
      Newpassword: ''

    }
  },
  methods: {
   
  }
    
}
</script>

 
<style lang="css" scoped></style>
<style>
.center {
  margin: 173px auto;
  width: 60%;
  border: 4px solid rgb(243, 95, 16);
  padding: 30px;
  padding-top: 100px;
  padding-bottom: 100px;

}
  .cancelbtn {

      margin: 0;
      position: absolute;
      text-align: center;
      top: 500px;
      left: 50%;
      width: 50%;
      padding: 7px 15px;
      -ms-transform: translate(-50%, -50%);
      transform: translate(-50%, -50%);
      background-color: rgb(243, 95, 16); 
    }
  .box {
    text-align: center;
    position: absolute;
     margin: -254px -34px;
     width: 60%;
    border-right: 4px solid rgb(243, 95, 16);
    border-left :4px solid rgb(243, 95, 16);
     border-top :4px solid rgb(243, 95, 16);
     border-bottom-color: 4px solid rgb(255, 255, 255);
     padding: 30px;
     padding-top: 30px;
     padding-bottom: 30px;

    }
    .Hw {
        background-color: rgb(255, 255, 255);
        position: absolute;
    }

</style>


