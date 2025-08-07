<template>

  <link href="https://fonts.googleapis.com/css2?family=Alfa+Slab+One&family=Orbitron&display=swap" rel="stylesheet">


  <header>
    <h1 class="heading">My Portfolio</h1>

    <div class="buttons">
      <a href="" class="contact">Contact</a>
      <a href="" class="project">Projects</a>
      <a href="" class="infoBtn">Info</a>
    </div>
  </header>

  <div class="body">


    <div class="portfolio">
      <div class="myInfo">
        <img :src="profileImage" alt="Profile image" class="profile-image" />

        <div class="text-content">
          <h3 class="greeting">Hi, I'm</h3>
          <h1 class="name">Sinethemba Mkhoma</h1>
          <h2 class="role">ICT Student</h2>

          <div class="icons">
            <a href="https://github.com/yourusername" target="_blank">
              <img src="@/assets/github.png" alt="GitHub" class="icon" />
            </a>
            <a href="https://linkedin.com/in/yourusername" target="_blank">
              <img src="@/assets/linkedin.png" alt="LinkedIn" class="icon" />
            </a>
          </div>
        </div>
      </div>
    </div>

    <div class="bottomBtns">
      <Button class="resume">Resume</Button>
      <Button class="contactInfo">Contact Info</Button>
    </div>

  </div>

</template>

<script>
export default {
  data() {
    return {
      profileImage: require('@/assets/profile.jpg')
    };
  }
};
</script>

<style>
html {
  background-color: rgb(209, 205, 196);
}

.body {
  background-image: url("/public/bgImage.png");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  height: 544px;
  z-index: 0;
  width: 100%;
  border-radius: 40px;
  padding-top: 30px;
}

header {
  position: relative;
  padding-top: 20px;
  background: linear-gradient(to bottom, rgba(22, 22, 22, 0.937), rgba(209, 205, 196));
  backdrop-filter: blur(50%);
  margin-top: -50px;
  margin-left: -8px;
  height: 170px;
  width: 100%;
  color: white;
}

.heading {
  letter-spacing: 2px;
  font-family: 'Obitron';
  font-size: 40px;
  margin-top: 70px;
  margin-left: 20px;
  text-align: center;
}


.myInfo {
  display: flex;
  align-items: center;
  gap: 40px;
  margin-top: 70px;
}

.portfolio {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 40px;
  color: white;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  font-weight: bolder;
  margin-top: 30px;
}

.profile-image {
  width: 200px;
  height: 200px;
  border-radius: 50%;
  object-fit: cover;
}

.text-content {
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.greeting {
  font-size: 20px;
  margin: 0;
}

.name {
  font-size: 35px;
  margin: 5px 0;
}

.role {
  font-size: 25px;
  margin-top: 5px;
}

.icons {
  margin-top: 20px;
  display: flex;
  gap: 20px;
}

.icon {
  width: 30px;
  height: 30px;
  transition: transform 0.3s ease;
}

.icon:hover {
  transform: scale(1.1);
}


.buttons {
  position: absolute;
  top: 30px;
  right: 40px;
  display: flex;
  gap: 20px;
}


.buttons a {
  margin-top: 60px;
  font-size: 16px;
  text-decoration: none;
  color: white;
  padding: 10px 20px;
  border-radius: 30px;
  background-color: rgba(255, 255, 255, 0.1);
  transition: transform 0.3s ease-in-out, background-color 0.3s;
}

.buttons a:hover {
  transform: translateY(-5px);
  background-color: rgba(255, 255, 255, 0.2);
}

.projects {
  text-align: center;
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
  padding-top: 10px;
  font-size: 40px;
}

.about {
  background: rgba(255, 255, 255, 0.2);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
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

.info {
  margin-top: 50px;
}

.content {
  margin-top: 10px;
}


.bottomBtns {
  justify-content: center;
  text-align: center;
  top: 30px;
  right: 40px;
  display: flex;
  gap: 20px;
  margin-top: 40px;
  margin-left: 110px;
  color: white;
  padding: 10px 20px;
  transition: transform 0.3s ease-in-out, background-color 0.3s;
}

.resume {
  background-color: rgba(77, 77, 77, 0.614);
  font-size: 16px;
  border-radius: 30px;
  color: white;
  width: 110px;
  height: 40px;
}

.contactInfo {
  background-color: rgba(77, 77, 77, 0.614);
  font-size: 16px;
  border-radius: 30px;
  color: white;
  width: 110px;
  height: 40px;
}

.contactInfo:hover {
  cursor: pointer;
  transition: ease-in-out 0.3s;
  transform: translateY(-5px);
  background-color: rgba(255, 255, 255, 0.2);
}

.resume:hover {
  cursor: pointer;
  transition: ease-in-out 0.3s;
  transform: translateY(-5px);
  background-color: rgba(172, 172, 172, 0.2);
}
</style>
