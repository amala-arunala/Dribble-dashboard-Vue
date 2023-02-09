<template>
  <div v-if="activeTab === 'TheDashboard'">
    <TheDashboard />
  </div>
  <div class="container" v-else-if="activeTab === 'UxDesign'">
    <div class="ux">
      <h1>UX</h1>
      <h1>DN</h1>
    </div>
    <h1 class="design">We design experiences.</h1>
    <button class="left-btn">
      <img
        src="../../assets/left-arrow.png"
        width="10px"
        height="10px"
        @click="clickHandler('TheDashboard')"
      />
    </button>
    <button class="right-btn">
      <img
        src="../../assets/right-arrow.png"
        width="10px"
        height="10px"
        @click="clickHandler('UxDesign')"
      />
    </button>
    <p class="emailid">HI@UXDN.CO</p>
  </div>
</template>

<script>
import TheDashboard from "./TheDashboard.vue";
export default {
  components: {
    TheDashboard,
  },
  data() {
    return {
      activeTab: "UxDesign",
    };
  },
  methods: {
    clickHandler(value) {
      this.activeTab = value;
    },
  },
};
</script>

<style scoped>
.container {
  width: 830px;
  height: 800px;
  margin-left: 300px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
  background-color: #1971c2;
  border-radius: 10px;
  position: relative;
  top: 0;
  left: 0;
  font-family: "Roboto", sans-serif;
}

.ux {
  border-radius: 50%;
  color: #1971c2;
  background-color: white;
  padding: 5px 30px;
  font-style: italic;
}

/* .ux h1 {
  line-height: 0.9;
} */

.design {
  color: white;
}

.emailid {
  color: white;
  border: none;
  padding: 2px 5px;
  background-color: #74c0fc;
  border-radius: 5px;
}

button {
  background-color: white;
  border-radius: 50%;
  border: none;
  overflow: visible;
}

.left-btn {
  position: absolute;
  left: 5%;
  top: 50%;
  transform: translate(-50%, -50%);
}

.right-btn {
  position: absolute;
  right: 5%;
  top: 50%;
  transform: translate(50%, -50%);
}

.left-btn:hover,
.right-btn:hover {
  background-color: white;
}
</style>
