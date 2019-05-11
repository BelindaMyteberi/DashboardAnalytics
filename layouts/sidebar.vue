<template>
  <div>
    <div class="topBar">
      <div class="admin">
        <div class="admin_img">
          <img src="../static/images/admin.png" width="35px">
        </div>
        <div class="admin_option" style="color:#414141; align-content: baseline">
          ADMINISTRATOR
        </div>
      </div>
      <div class="icon-header">
        <div class="menu_img">
          <img src="../assets/sass/svg/menu.svg" alt="menu">
        </div>
        <div class="search_img">
          <img src="../assets/sass/svg/search.svg" alt="search">
        </div>
        <div class="bell_img">
          <img src="../assets/sass/svg/bell.svg" alt="bell">
        </div>
        <div class="envelope_img">
          <img src="../assets/sass/svg/envelope.svg" alt="envelope">
        </div>
      </div>
    </div>
    <div class="main-container">
      <div class="sidebar">
        <div class="dashboard">
          <div class="img-holder bela">
            <img src="../assets/sass/svg/home.svg" alt="home">
          </div>
          <div class="dashboard_option">
            <nuxt-link :to="{name:'dashboard'}" style="text-decoration: none">
              <p>
                Dashboard
              </p>
            </nuxt-link>
          </div>
        </div>

        <div class="email">
          <div class="img-holder">
            <img src="../assets/sass/svg/email.svg" alt="email">
          </div>
          <div class="email_option">
            <nuxt-link :to="{name:'email'}" style="text-decoration: none">
              <p>
                Email
              </p>
            </nuxt-link>
          </div>
        </div>

        <div class="compose">
          <div class="img-holder">
            <img src="../assets/sass/svg/compose.svg" alt="compose">
          </div>
          <div class="compose_option">
            <nuxt-link :to="{name:'compose'}" style="text-decoration: none">
              <p>
                Compose
              </p>
            </nuxt-link>
          </div>
        </div>
        <div class="calendar">
          <div class="img-holder">
            <img src="../assets/sass/svg/calendar.svg" alt="email">
          </div>
          <div class="calendar_option">
            <nuxt-link :to="{name:'calendar'}" style="text-decoration: none">
              <p>
                Calendar
              </p>
            </nuxt-link>
          </div>
        </div>
        <div class="chat">
          <div class="img-holder">
            <img src="../assets/sass/svg/chat.svg" alt="chat">
          </div>
          <div class="chat_option">
            <nuxt-link :to="{name:'chat'}" style="text-decoration: none">
              <p>
                Chat
              </p>
            </nuxt-link>
          </div>
        </div>
        <div class="charts">
          <div class="img-holder">
            <img src="../assets/sass/svg/charts.svg" alt="charts">
          </div>
          <div class="charts_option">
            <nuxt-link :to="{name:'chart'}" style="text-decoration: none">
              <p>
                Chart
              </p>
            </nuxt-link>
          </div>
        </div>
        <div class="form">
          <div class="img-holder">
            <img src="../assets/sass/svg/form.svg" alt="form">
          </div>
          <div class="form_option">
            <nuxt-link :to="{name:'form'}" style="text-decoration: none">
              <p>
                Form
              </p>
            </nuxt-link>
          </div>
        </div>

      </div>
      <div class="container-of-page">
        <nuxt/>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
  .topBar{
    height:50px;
    display: flex;
    flex-direction: row;
    border-bottom:#F7F7F7 solid 5px;
  }
  .admin{
    padding:0px 10px;
    text-align: center;
    width:200px;
    height: 50px;
    display: flex;
    flex-direction:row;
    border-right:solid 5px #F7F7F7;
    .admin_img{
      width:35px;
      height:20px;
      padding-right: 5px;
      margin:5px;
     img{
      border-radius: 50%;
      }
    }
    .admin_option{
      text-align: center;
      padding: 10px;
    }
  }
  .icon-header {
    display: flex;
    justify-content: center;
    box-sizing: border-box;
    .menu_img, .search_img, .bell_img, .envelope_img {
      width:15px;
      height:15px;
    }
  }

  .main-container {
    display: flex;

    .container-of-page {
      width: calc(100% - 205px);
    }
  }

  .sidebar {
    width: 200px;
    height: 100vh;
    display: inline-flex;
    flex-direction: column;
    background: #FFFFFF;
    color:#B0B2B4;
    border-right: #F7F7F7 solid 5px;
    padding: 10px;
  }

  .dashboard, .email, .calendar, .charts, .chat, .compose, .form {
    display: flex;
    flex-direction: row;
    align-content: space-between;
    width: 200px;
    font-size: 16px;
    padding: 5px 15px;
  }

  .img-holder {
    width: 15px;
    height: 15px;
    position: relative;
    margin-right:10px;
    img {
      width: 100%;
      height: 100%;
    }
  }

</style>


