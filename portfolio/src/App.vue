<template>

  <header>

    <div class="info">
      <h1 class="name">Sinethemba Mkhoma</h1>
      <h2 class="role">ICT Student</h2>
    </div>

    <div class="button">
      <Button class="contact">Contact</Button>
    </div>

  </header>

  <div class="body">

    <div class="portfolio">
      <h1>My Portfolio</h1>
    </div>

    <section class="about">
      <div class="bgImage">

      </div>
      <h2 class="aboutMe">About Me</h2>
      <p class="abt">
        "I am a passionate 2nd year student who is good at making figma projects and I can code a webisite from the
        ground
        up using vue, html and css"
      </p>
    </section>

    <section class="projects">
      <h2 class="myProjects">My Projects</h2>
    </section>
  </div>


</template>

<script>

</script>

<style>
html {
  background-color: rgb(209, 205, 196);
}

.body {
  background-image: url("/public/bgImage.jpg");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  height: 500px;
  z-index: 0;
  border-radius: 40px;
  padding-top: 30px;
  margin-top: 50px;
}

header {
  padding-top: 20px;
  background: linear-gradient(to bottom, rgba(22, 22, 22, 0.937), rgba(209, 205, 196));
  backdrop-filter: blur(50%);
  margin-top: -50px;
  margin-left: -8px;
  height: 200px;
  width: 1536px;
  color: white;
}

.portfolio {
  text-align: center;
  color: white;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  font-weight: bolder;
}

.contact {
  margin-left: 90%;
  margin-top: -50px;
  text-align: center;
  width: 110px;
  height: 45px;
  border-radius: 30px;
  background-color: white;
  color: black;
  z-index: 1;
}

.projects {
  padding-top: -10px;
  text-align: center;
  background-color: rgba(255, 255, 255, 0.422);
  color: black;
  width: 40%;
  height: 350px;
  border-radius: 70px;
  margin-left: 55%;
  margin-top: -350px;
  background: rgba(255, 255, 255, 0.2);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.3);
  color: white;

}

.myProjects {
  padding-top: 40px;
  font-size: 40px;
}

.about {
  background: rgba(255, 255, 255, 0.2);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border-radius: 15px;
  border: 1px solid rgba(255, 255, 255, 0.3);
  color: white;
  padding-top: 10px;
  text-align: center;
  background-color: rgba(255, 255, 255, 0.356);
  width: 40%;
  height: 330px;
  border-radius: 70px;
  margin-top: 40px;
  margin-left: 70px;
}

.aboutMe {
  margin-top: 25px;
  font-size: 40px;
}

.abt {
  margin-top: 30px;
  font-size: 20px;
}

.name {
  font-size: 40px;
  margin-top: -20px;
  margin-left: 10px;
  color: white;
}

.info {
  margin-top: 50px;
}

.button {
  margin-top: -80px;
}

.role {
  font-size: 25px;
  text-align: left;
  margin-left: 10px;
  color: white;
  margin-top: 0;
}

.content {
  margin-top: 10px;
}
</style>
