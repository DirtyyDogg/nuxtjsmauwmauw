<template>
  <section>
    <!-- <p>hier gaat de app beginnen</p> -->
    <b-navbar toggleable="md" type="dark" variant="dark">
      <b-navbar-brand to="/">
        Navbar
      </b-navbar-brand>
      <b-navbar-toggle target="navbar-toggle-collapse">
        <template v-slot:default="{ expanded }">
          <b-icon v-if="expanded" icon="chevron-bar-up" />
          <b-icon v-else icon="chevron-bar-down" />
        </template>
      </b-navbar-toggle>
      <!--  -->
      <b-collapse id="navbar-toggle-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item to="#">
            Link1
          </b-nav-item>
          <b-nav-item to="#">
            Link2
          </b-nav-item>
          <b-nav-item to="#" disabled>
            Disabled
          </b-nav-item>
          <b-nav-item-dropdown text="Lang" right>
            <b-dropdown-item href="#">
              EN
            </b-dropdown-item>
            <b-dropdown-item href="#">
              ES
            </b-dropdown-item>
            <b-dropdown-item href="#">
              RU
            </b-dropdown-item>
            <b-dropdown-item href="#">
              FA
            </b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
        <b-navbar-nav class="ml-auto">
          <b-nav-item-dropdown text="Lang" right>
            <b-dropdown-item href="#">
              EN
            </b-dropdown-item>
            <b-dropdown-item href="#">
              ES
            </b-dropdown-item>
            <b-dropdown-item href="#">
              RU
            </b-dropdown-item>
            <b-dropdown-item href="#">
              FA
            </b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
    <!--  -->
    <div class="App">
      <div class="een">
        <h1>okee</h1>
        <div class="twee">
          <h1>Niet okee</h1>
          <div class="container" style="margin-top:30px;">
            <div class="row">
              <div class="col-sm-4">
                <h1>Waar hadden we het over???</h1>
              </div> <!-- einde col-sm-4 -->
              <h1>UGHHH NEVERMIND!</h1>
            </div> <!-- einde row -->
          </div> <!-- einde container -->
        </div> <!-- einde class 2 -->
      </div> <!-- einde 1  -->
      <section id="twee">
        <div class="drie">
          <div class="jumbotron text-center" style="margin:0 0 0;position:absolute;bottom:0;overflow-y:auto;padding:4px 0 1px 0;border: black 1px solid; width: 100%; min-width: 310px; max-width:1475px;">
            <p>Footer</p>
          </div>
        </div> <!-- einde 3 -->
      </section> <!-- einde section 2 -->
    </div> <!-- einde app -->
  </section>
</template>
<script>

</script>
<style>
.drie {
    position: absolute;
    margin-bottom: 0px;
    bottom: 0;
    min-width: 500px;
    max-width: 1434px;
    width: 100%
}
h1 {
    font-size: 1.5rem;
}
</style>
