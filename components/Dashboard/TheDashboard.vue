<template>
  <div>
    <div class="outer" v-if="activeTab === 'TheDashboard'">
      <div class="inner">
        <div class="sidebar">
          <TheSidebar />
          <div>
            <MainPart />
          </div>
        </div>
      </div>

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
    </div>
    <div v-else-if="activeTab === 'UxDesign'">
      <UxDesign />
    </div>
    <div class="images">
      <img
        src="../../assets/dashboard1.png"
        width="100px"
        height="80px"
        :style="{ 'margin-right': '10px' }"
        @click="clickHandler('TheDashboard')"
      />
      <img
        src="../../assets/dashboard2.png"
        width="100px"
        height="80px"
        @click="clickHandler('UxDesign')"
      />
    </div>
  </div>
</template>

<script>
import MainPart from "./MainPart.vue";
import TheSidebar from "./TheSidebar.vue";
import UxDesign from "./UxDesign.vue";
export default {
  components: {
    TheSidebar,
    MainPart,
    UxDesign,
  },
  data() {
    return {
      activeTab: "TheDashboard",
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
.outer {
  width: 830px;
  height: 800px;
  margin-left: 300px;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: black;
  border-radius: 10px;
  position: relative;
  top: 0;
  left: 0;
}

.inner {
  width: 750px;
  height: 730px;
  border-radius: 10px;
  overflow: hidden;
  background-color: white;
}

.sidebar {
  width: 50px;
  height: 730px;
  background-color: #f1f3f5;
  display: flex;
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

.images {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 40px;
  cursor: pointer;
  border-radius: 10px;
}
</style>
