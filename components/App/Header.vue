<template>
  <section class="app-header">
    <b-navbar id="secrimento" toggleable="lg" type="dark" variant="dark" fixed>
      <b-navbar-brand id="secrimento-brand" to="/">
        {{ SiteTitle }}
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse">
        <template v-slot:default="{ expanded }">
          <b-icon v-if="expanded" icon="chevron-bar-up" />
          <b-icon v-else icon="chevron-bar-down" />
        </template>
      </b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav style="">
        <b-navbar-nav>
          <!--  -->
          <b-nav-item to="/over/ons">
            Over ons
          </b-nav-item>
          <b-nav-item to="/projecten">
            Projecten
          </b-nav-item>
          <b-nav-item to="/gallerij">
            Gallerij
          </b-nav-item>
          <b-nav-item-dropdown text="Contact" right>
            <b-dropdown-item>
              0800 - 1234
            </b-dropdown-item>
            <b-dropdown-item to="/contact">
              Contact formulier
            </b-dropdown-item>
            <b-dropdown-item to="/contact/chat">
              *New Chat?
            </b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
        <b-navbar-nav class="ml-auto">
          <b-nav-form>
            <b-form-input size="sm" class="mr-sm-2" style="background-color:#222323b5; color: black; border: 1px solid #3b8070;" placeholder="Search" />
            <b-button size="sm" class="my-2 my-sm-0" style="background: #3b8070;" type="submit">
              Zoeken
            </b-button>
          </b-nav-form>
          <!-- old -->
          <div>
            <b-nav-item-dropdown v-if="user" text="User" right>
              <b-dropdown-item href="#">
                Mijn Profiel
              </b-dropdown-item>
              <b-dropdown-item href="#">
                Admin Panel
              </b-dropdown-item>
              <b-dropdown-item href="#">
                Uitloggen
              </b-dropdown-item>
            </b-nav-item-dropdown>
            <div v-else>
              <b-nav-item-dropdown v-if="!user" text="Niet ingelogd" right>
                <b-dropdown-item to="/users/login">
                  Login
                </b-dropdown-item>
                <b-dropdown-item to="/users/registratie">
                  Register
                </b-dropdown-item>
              </b-nav-item-dropdown>
            </div>
          </div>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </section>
</template>

<script>
//
export default {
  data () {
    return {
      SiteTitle: 'MauwMauw',
      user: false
    }
  }
}
</script>

<style>
/* 600px */
 @media screen and (max-width: 993px) {
     ul.dropdown-menu.dropdown-menu-right.show {
        text-align: center;
    }
    .form-inline {
        justify-content: center;
    }
 }

.navbar {
    top: 0px;
}
nav#secrimento {
    background: linear-gradient(179deg, #353535, #040303);
}
/* form.control {
    color: #c5c5c5;
    border-color: #80bdff;
    box-shadow: 0 0 0 0.2rem rgba(0, 123, 255, 0.25);
    #3b8070;

} */

.dropdown-menu {
    color: #83a90f;
    background: #1a1b1a;
}
.dropdown-item {
    color: #a6a8ab;
}
.dropdown-item:hover, .dropdown-item:focus {
    color: #e6e6e6;
    text-decoration: none;
    background-color: #3b807070
}
/** INPUT */
input, select, textarea, form-control, ::placeholder {
    color: #3b8070 !important;
}
/* input::placeholder {
    color: aqua;
} */
form.control:focus {
    color: #c5c5c5;
    border-color: #80bdff;
    box-shadow: 0 0 0 0.2rem rgba(0, 123, 255, 0.25);

}
</style>
