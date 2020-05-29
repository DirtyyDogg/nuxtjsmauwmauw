<template>
  <section id="services" class="services pt-100 pb-500">
    <b-container id="Services" class="ContainerServices container">
      <b-row>
        <div class="col-xl-6 mx-auto text-center">
          <div class="section-title mb-100">
            <p>what i can do</p>
            <h4>my services</h4>
          </div>
        </div>
      </b-row>
      <!--  -->
      <b-row cols="1" cols-sm="2" cols-md="3" cols-lg="3" class="text-center">
        <b-col>
          <Service1 />
        </b-col>
        <b-col>
          <Service2 />
        </b-col>
        <b-col>
          <Service3 />
        </b-col>
        <b-col>
          <Service4 />
        </b-col>
        <b-col>
          <Service5 />
        </b-col>
        <b-col>
          <Service6 />
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
import Service1 from '~/components/ServicesBox/service1'
import Service2 from '~/components/ServicesBox/service2'

import Service3 from '~/components/ServicesBox/service3'
import Service4 from '~/components/ServicesBox/service4'
import Service5 from '~/components/ServicesBox/service5'
import Service6 from '~/components/ServicesBox/service6'
export default {
  components: {
    Service1, Service2, Service3, Service4, Service5, Service6
  }
}
</script>

<style lang="scss">
div#Services.ContainerServices.container {
    /* background: aliceblue; */
    margin-top: -33px;
}
div#Services.ContainerServices.container .row {
    margin: 0 0 -83px 0;
}

// // // Section \\ \\ \\
.services {
    background-color: #0404044d;
}
.section-title {
    position: relative
}
.pt-100 {
    padding-top: 100px;
}
.pb-100 {
    padding-bottom: 100px;
}
.mb-100{
    margin-bottom:100px;
}

// Section-title h4
.section-title h4 {
    font-size: 40px;
    font-weight: 600;
    text-transform: capitalize;
    position: relative;
    padding-bottom: 20px;
    display: inline-block;
    color: #a8f39b;
}
.section-title h4:before {
    position: absolute;
    content: "";
    width: 80px;
    height: 2px;
    background-color: #d8d8d8;
    bottom: 0;
    left: 50%;
    margin-left: -40px;
}
.section-title h4:after {
    position: absolute;
    content: "";
    width: 50px;
    height: 2px;
    background-color: #FF7200;
    left: 0;
    bottom: 0;
    left: 50%;
    margin-left: -25px;
}
// Section-tilte h4 \\

// Section-title p
.section-title p {
    font-size: "16px";
    margin-bottom: 5px;
    font-weight: 400;
    color: rgba(0, 247, 190, 0.52);
}
// Section-title p \\

// // // Single-Services \\ \\ \\

// single-service
.single-service {
    position: relative;
    text-align: center;
    margin-bottom: 50px;
    -webkit-transition: .3s;
    transition: .3s;
    padding: 30px 20px;
    box-shadow: 0 1px 4px rgba(0, 0, 0, 0.16)
}
// \\
// single-service before
.single-service:before {
    position: absolute;
    width: 0;
    height: 0;
    background-color: #a8f39b;
    left: 0;
    top: 0;
    content: "";
    -webkit-transition: .3s;
    transition: .3s
}
// \\
// single-service after
// color: #3f4040b0;
// text-shadow: 0px 1px 1px #ffffffa6;
.single-service:after {
    position: absolute;
    width: 0;
    height: 0;
    background-color: #098a6cb0;
    right: 0;
    bottom: 0;
    content: "";
    -webkit-transition: .3s;
    transition: .3s
}
// && hover
.single-service:hover:after,
.single-service:hover:before {
    width: 50%;
    height: 2px;
    -webkit-transition: .3s;
    transition: .3s
}
.single-service:hover {
    box-shadow: 1px 3px 10px 0 rgba(0, 0, 0, 0.10)
}
// \\ \\

// //   single-service texture
.single-service h4 {
    font-size: 20px;
    font-weight: 400;
    margin-bottom: 15px;
    text-transform: capitalize;
    color: #098a6c;
    text-shadow: 0px 1px 1px #000000;
}
.single-service p {
    font-size: 15px;
    line-height: 1.8;
    color: #90f193;
    text-shadow: 0px 1px 1px #000000;
}
// \\
// Einde textures \\

// //   single-service Icons
.single-service i.fa {
    font-size: 20px;
    width: 60px;
    height: 60px;
    border: 1px solid #ddd;
    line-height: 60px;
    margin-bottom: 30px;
    border-radius: 50%;
    -webkit-transition: .3s;
    transition: .3s
}
.single-service:hover i.fa {
    background-color: #FF7200;
    color: #fff;
    border-color: #FF7200;
    border-radius: 0;
}
// \\
</style>
