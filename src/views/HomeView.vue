<template>
  <div class="home">
    <Nav />
    <div class="home-view">
      <div class="home-a">
        <h3>
          Mars digital creation is a <span>design</span> and large format
          printing company based in <span>Nairobi,kenya</span>
        </h3>
      </div>
      <div class="home-b">
        <span class="home-mid-img">
          <img src="../assets/design.jpg" alt="middle img" class="mid-img" />
        </span>
      </div>
    </div>
    <div>
      <Client />
    </div>
    <div>
      <div class="service">
        <h3>service</h3>
        <h1>check out our service offered</h1>
        <Service />
      </div>
      <div class="project">
        <h3>project</h3>
        <h1>Enjoy the show</h1>
        <ProjectCard />
      </div>
      <div>
        <Done />
      </div>
      <div>
        <Contact />
      </div>
    </div>
  </div>
</template>
<script>
import Nav from "../components/NavBar.vue";
import Service from "../views/ServiceView.vue";
import Contact from "../views/ContactView.vue";
import Done from "../components/projectsDone.vue";
import Client from "../components/ClientComponent.vue";
import ProjectCard from "../components/ProjectCard.vue";

export default {
  components: {
    Nav,
    Done,
    Client,
    Contact,
    Service,
    ProjectCard,
  },
};
</script>
<style>
@import "../style/HomeView.css";
</style>
