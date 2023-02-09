<template>
  <div class="header">
    <div class="nav-items">
      <img src="../assets/logo.png" alt="logo" width="100px" height="100px" />

      <div class="dropdown">
        <a href="#" class="dropbtn">Inspiration</a>
        <div class="dropdown-content">
          <ul v-for="list in lists" :key="list.type">
            <li>
              <div class="list-img">
                <img
                  :src="require(`../assets/${list.img}`)"
                  width="30px"
                  height="30px"
                  class="first"
                />
                <div class="list-heading">
                  <h6 class="list-type">{{ list.type }}</h6>
                  <p class="list-desc">{{ list.description }}</p>
                </div>
                <img
                  src="../assets/right-arrow-48.png"
                  width="15px"
                  height="15px"
                  class="second"
                />
              </div>
            </li>
          </ul>
        </div>
      </div>

      <div class="dropdown">
        <a href="#" class="dropbtn">Find Work</a>
        <div class="dropdown-content">
          <ul v-for="list in list2" :key="list.type">
            <li>
              <div class="list-img">
                <img
                  :src="require(`../assets/${list.img}`)"
                  width="30px"
                  height="30px"
                  class="first"
                />
                <div class="list-heading">
                  <h6 class="list-type">{{ list.type }}</h6>
                  <p class="list-desc">{{ list.description }}</p>
                </div>
                <img
                  src="../assets/right-arrow-48.png"
                  width="15px"
                  height="15px"
                  class="second"
                />
              </div>
            </li>
          </ul>
        </div>
      </div>

      <div class="dropdown">
        <a href="#" class="dropbtn">Learn Design</a>
        <div class="dropdown-content">
          <ul v-for="list in list3" :key="list.type">
            <li>
              <div class="list-img">
                <img
                  :src="require(`../assets/${list.img}`)"
                  width="30px"
                  height="30px"
                  class="first"
                />
                <div class="list-heading">
                  <h6 class="list-type">{{ list.type }}</h6>
                  <p class="list-desc">{{ list.description }}</p>
                </div>
                <img
                  src="../assets/right-arrow-48.png"
                  width="15px"
                  height="15px"
                  class="second"
                />
              </div>
            </li>
          </ul>
        </div>
      </div>

      <div class="dropdown">
        <a href="#" class="dropbtn">Go Pro</a>
        <div class="dropdown-content">
          <ul v-for="list in list4" :key="list.type">
            <li>
              <div class="list-img">
                <img
                  :src="require(`../assets/${list.img}`)"
                  width="30px"
                  height="30px"
                  class="first"
                />
                <div class="list-heading">
                  <h6 class="list-type">{{ list.type }}</h6>
                  <p class="list-desc">{{ list.description }}</p>
                </div>
                <img
                  src="../assets/right-arrow-48.png"
                  width="15px"
                  height="15px"
                  class="second"
                />
              </div>
            </li>
          </ul>
        </div>
      </div>

      <div class="dropdown">
        <a href="#" class="dropbtn">Hire Designers</a>
        <div class="dropdown-content">
          <ul v-for="list in list5" :key="list.type">
            <li>
              <div class="list-img">
                <img
                  :src="require(`../assets/${list.img}`)"
                  width="30px"
                  height="30px"
                  class="first"
                />
                <div class="list-heading">
                  <h6 class="list-type">{{ list.type }}</h6>
                  <p class="list-desc">{{ list.description }}</p>
                </div>
                <img
                  src="../assets/right-arrow-48.png"
                  width="15px"
                  height="15px"
                  class="second"
                />
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div class="button">
      <img
        src="../assets/search.png"
        alt="logo"
        width="20px"
        height="20px"
        class="search-icon"
      />
      <p class="signin-btn">Sign in</p>
      <p class="signup-btn">Sign up</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      lists: [
        {
          img: "windows.png",
          type: "Explore Design Work",
          description: "Trending designs to inspire you",
        },
        {
          img: "icons8-favorite-30.png",
          type: "New & Noteworthy",
          description: "Up-and-coming designers",
        },
        {
          img: "square.png",
          type: "Playoffs",
          description: "Work designers are riffling on",
        },
        {
          img: "notepad.png",
          type: "Blog",
          description: "Interviews, tutorials, and more",
        },
        {
          img: "reminder.png",
          type: "Weekly Warmup",
          description: "Prompt to flex your design skills",
        },
      ],
      list2: [
        {
          img: "reminder.png",
          type: "Job Board",
          description: "Find your dream design job",
        },
        {
          img: "tea-cup.png",
          type: "Freelance Projects",
          description: "An exclusive list for contract work",
        },
        {
          img: "mail.png",
          type: "Want freelance design projects?",
          description: "Get new leads in your inbox every day",
        },
        {
          img: "contact.png",
          type: "Personalize your profile with video",
          description: "Introduce yourself to new clients with Pitch",
        },
      ],
      list3: [
        {
          img: "stationery.png",
          type: "Certified Product Design Course",
          description: "Learn product design in just 16 weeks...",
        },
        {
          img: "curriculum.png",
          type: "Introduction to UI Design",
          description: "Learn UI Design Basics and Figma Fundamentals...",
        },
        {
          img: "services.png",
          type: "Design Systems Course",
          description: "Scale Design Systems in 8 weeks...",
        },
        {
          img: "archery.png",
          type: "Design Career Prep Course",
          description:
            "Land your dream job! You'll have a career support specialist to review your portfolio...",
        },
        {
          img: "video-cam.png",
          type: "Browse our courses & workshops",
          description:
            "Level up your skills with our interactive courses and workshops...",
        },
      ],
      list4: [
        {
          img: "deltohedron.png",
          type: "For Designers",
          description: "Portfolio creation made easy",
        },
        {
          img: "pencil-cup.png",
          type: "For Freelancers",
          description: "Fresh leads in your inbox every day",
        },
        {
          img: "team.png",
          type: "For Teams",
          description: "Build your team's pipeline or profile",
        },
      ],
      list5: [
        {
          img: "small-hearts.png",
          type: "Designer Search",
          description: "Find, contact, and hire designers",
        },
        {
          img: "plus-red.png",
          type: "List my Job Opening",
          description: "The #1 job board for creatives",
        },
        {
          img: "plus-green.png",
          type: "Post a Freelance Project",
          description: "Board for freelance and contract work",
        },
      ],
    };
  },
};
</script>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-family: "Roboto", sans-serif;
}

.nav-items {
  display: flex;
  justify-content: start;
  align-items: center;
}

.dropdown {
  position: relative;
  display: inline-block;
}

.dropbtn {
  border: none;
  margin-bottom: 50px;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: white;
  min-width: 400px;
  box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
  border-radius: 10px;
  z-index: 1;
  padding-top: 20px;
}

.dropdown:hover .dropdown-content {
  display: block;
}

a {
  text-decoration: none;
  color: black;
  margin-right: 20px;
}

.list-img {
  display: flex;
  justify-content: flex-start;
}

.list-type {
  cursor: pointer;
}

.first {
  cursor: pointer;
}

.second {
  display: none;
  margin-top: 15px;
  margin-left: 50px;
}

.first:hover + .second {
  display: block;
}

.list-heading:hover + .second {
  display: block;
}

/* .list-img:hover {
  border: 1px solid #cc5de8;
} */

.list-desc {
  font-size: 13px;
}

.list-heading {
  margin-left: 20px;
  line-height: 0.75;
  cursor: pointer;
}

li {
  list-style-type: none;
}

/* li :first-child {
  margin-top: 25px;
} */

.button {
  display: flex;
}

.search-icon {
  margin-right: 10px;
  font-weight: 100;
  margin-top: 24px;
}

.signin-btn {
  margin-right: 10px;
  margin-top: 24px;
  font-size: 18px;
  cursor: pointer;
  font-weight: 300;
}

.signup-btn {
  font-size: 17px;
  font-weight: 500;
  margin-top: 15px;
  border: none;
  border-radius: 7px;
  padding: 5px 10px;
  background-color: #f06595;
  color: white;
  cursor: pointer;
  margin-right: 10px;
}
</style>
