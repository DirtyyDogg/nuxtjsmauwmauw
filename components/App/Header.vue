<template>
  <section class="app-header">
    <b-navbar id="secrimento" toggleable="lg" type="dark" variant="dark" fixed>
      <b-navbar-brand id="secrimento-brand" href="#">
        NavBar
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse">
        <template v-slot:default="{ expanded }">
          <b-icon v-if="expanded" icon="chevron-bar-up" />
          <b-icon v-else icon="chevron-bar-down" />
        </template>
      </b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item href="#">
            Link
          </b-nav-item>
          <b-nav-item href="#">
            Disabled
          </b-nav-item>
        </b-navbar-nav>
        <b-navbar-nav class="ml-auto">
          <b-nav-form>
            <b-form-input size="sm" class="mr-sm-2" style="background-color:#222323b5; color: black; border: 1px solid #3b8070;" placeholder="Search" />
            <b-button size="sm" class="my-2 my-sm-0" style="background: #3b8070;" type="submit">
              Zoeken
            </b-button>
          </b-nav-form>
          <b-nav-item-dropdown text="Lang" right>
            <b-dropdown-item href="#">
              1
            </b-dropdown-item>
            <b-dropdown-item href="#">
              2
            </b-dropdown-item>
            <b-dropdown-item href="#">
              3
            </b-dropdown-item>
          </b-nav-item-dropdown>
          <b-nav-item-dropdown right>
            <template v-slot:button-content>
              <em>User</em>
            </template>
            <b-dropdown-item href="#">
              Profile
            </b-dropdown-item>
            <b-dropdown-item href="#">
              Loguit
            </b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </section>
</template>

<style>
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
