<template>
  <div>
    <div class="container">
      <div class="pop_up">
        <div class="title" >
          <h3>Log In</h3>
        </div>

        <div class="email_password_submit_container">
          <input type="text" name="email" id="email" v-model="valueOfInputEmail" placeholder="Email">
                        <!--<img src="../assets/sass/svg/home.svg" alt="">-->
            <input type="text" name="password" id="password" v-model="valueOfInputPassword" placeholder="Password">
          <div class="button_holder">
            <button class="signInBtn" @click="validate"> Submit</button>
          </div>
          </div>
        </div>
      <!--<div class="welcome_pop_up" v-if="!seen">
       <p> Welcome </p>
        <p> {{valueOfInputEmail}}</p>
        </div>-->
    </div>

  </div>
</template>
<script>
  export default {
    data() {
      return {
        valueOfInputEmail:'',
        valueOfInputPassword:'',
        filled: false,
        username:'',
        admin_email:'belinda',
        admin_password:'bela',
      }
    },
    methods: {
      //hide(){
       // this.seen=false;
     //}
      validate(){
        //if(this.valueOfInputEmail!=null && this.valueOfInputPassword!=null){
        //  this.filled=true;
        if(this.valueOfInputEmail===this.admin_email && this.valueOfInputPassword===this.admin_password){
            window.location.href = '/dashboard';
        }
        else
          window.location.href = '/signin';
      }
    }
  }


</script>
