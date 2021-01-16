<template>
  <navbar id="warning" light>
Amalitech Front-Desk Portal
    <!-- <mdb-navbar-toggler>
      <mdb-navbar-nav>
        <mdb-nav-item href="#" active>Home</mdb-nav-item>
        <mdb-nav-item href="#">Features</mdb-nav-item>
        <mdb-nav-item href="#">Pricing</mdb-nav-item>
        <mdb-dropdown tag="li" class="nav-item">
          <mdb-dropdown-toggle tag="a" navLink color="warning" slot="toggle" waves-fixed>Dropdown</mdb-dropdown-toggle>
        </mdb-dropdown>
      </mdb-navbar-nav>
      <form>
        <mdb-input type="text" class="text-white" placeholder="Search" aria-label="Search" label navInput waves waves-fixed/>
      </form>
    </mdb-navbar-toggler> -->
  </navbar>
</template>

<style scoped>
#warning {
  display: inline-block;
  background-color: #690009;
  height: 55px;
  width: 1200%; 
  padding: 10px 0 0 370px ;
  padding-right: 100px;
  color: #ffa33b;
  align-items: left;
  max-width: 120%;
}
#warning{
  font-size: 40px;
  color: rgb(235, 209, 126);
  text-align: justify;
  -webkit-animation: glow 2s ease-in-out infinite alternate;
  -moz-animation: glow 1s ease-in-out infinite alternate;
  animation: glow 3s ease-in-out infinite alternate;
}

@-webkit-keyframes glow {
  from {
    text-shadow: 0 0 10px rgb(243, 213, 162), 0 0 20px rgb(53, 50, 21), 0 0 30px #e69600, 0 0 40px #e68200, 0 0 50px #e6a900, 0 0 60px #e6bc00, 0 0 70px #faa031;
  }
  to {
    text-shadow: 0 0 20px rgb(235, 188, 59), 0 0 30px #ffed4d, 0 0 40px #ffc14d, 0 0 50px #ffe44d, 0 0 60px #ff4da6, 0 0 70px #ff4da6, 0 0 80px #ff4da6;
  }
}

footer ul{
  list-style: none;
  padding: 2px;
}
footer ul li{
  display: inline-block;
  margin: 0px 50px;
}

mdb-nav-item {
  display: inline-block;
  padding: 20px;
}
</style>