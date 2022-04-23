<template>
  <div class="home">
    <Nav ref="nav" />
    <div class="home-view" ref="homeView">
      <div class="home-a" ref="homeA">
        <h3>
          Mars digital creation is a <span>design</span> and large format
          printing company based in <span>Nairobi,kenya</span>
        </h3>
      </div>
      <div class="home-b" ref="homeB">
        <span class="home-mid-img">
          <img src="../assets/mars.jpg" alt="middle img" class="mid-img" />
        </span>
      </div>
    </div>
    <div ref="client">
      <Client />
    </div>
    <div>
      <div class="service" ref="service">
        <h3>service</h3>
        <h1>check out our service offered</h1>
        <Service />
      </div>
      <div class="project" ref="project">
        <h3>project</h3>
        <h1>Enjoy the show</h1>
        <ProjectCard />
      </div>
      <div ref="done">
        <Done />
      </div>
      <div ref="comment">
        <Comment />
      </div>
      <div ref="contact">
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
import Comment from "../components/CommentComponent.vue";
export default {
  components: {
    Nav,
    Done,
    Client,
    Service,
    Contact,
    Comment,
    ProjectCard,
  },
};
</script>
<style>
@import "../style/HomeView.css";
</style>
