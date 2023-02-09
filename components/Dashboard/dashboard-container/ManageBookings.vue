<template>
  <div class="grid-3-cols">
    <div class="satisfaction">
      <p class="heading">Satisfaction rate</p>
      <div class="rate">
        <h4>75%</h4>
        <img src="../../../assets/sort-up.png" width="20px" height="20px" />
        <p>3%</p>
      </div>

      <div class="emojis">
        <div class="emoji1">
          <img src="../../../assets/smile.png" width="20px" height="20px" />
          <h6>12</h6>
        </div>
        <div class="emoji2">
          <img
            src="../../../assets/face-with-raised-eyebrow.png"
            width="30px"
            height="30px"
          />
          <h6>1</h6>
        </div>
        <div class="emoji3">
          <img src="../../../assets/sad.png" width="20px" height="20px" />
          <h6>2</h6>
        </div>
      </div>
      <div class="tasks">
        <p class="heading">Urgent & vip tasks</p>
        <div class="tasks-info">
          <div class="room-info">
            <p>Clean up room</p>
            <p>Room 103</p>
          </div>
          <img
            src="../../../assets/icons8-cat-profile-48.png"
            alt="profile"
            width="20px"
            height="20px"
          />
        </div>
        <hr />

        <div class="tasks2-info">
          <div class="room2-info">
            <p>Change linen, clean windows</p>
            <p>Villa 1<span>vip</span></p>
          </div>
          <img
            src="../../../assets/icons8-cat-profile-48.png"
            alt="profile"
            width="20px"
            height="20px"
          />
        </div>
        <hr />

        <div class="tasks-info">
          <div class="room-info">
            <p>Clean up room</p>
            <p>Room 102</p>
          </div>
          <img
            src="../../../assets/icons8-cat-profile-48.png"
            alt="profile"
            width="20px"
            height="20px"
          />
        </div>
        <p class="all-tasks">SEE ALL TASKS</p>
      </div>
    </div>
    <div class="col2">
      <div class="col2-heading">
        <p class="booking">Bookings</p>
        <p class="manage">MANAGE BOOKINGS</p>
      </div>
      <div class="barchart">
        <BarChart
          :options="options"
          :width="width"
          :height="height"
          xlabel="Year"
          ylabel="Prices($)"
        />
      </div>
    </div>
    <div class="col3">
      <h6>New Guests</h6>
      <div class="rate">
        <h4>24</h4>
        <img src="../../../assets/sort-up.png" width="20px" height="20px" />
        <p>32%</p>
      </div>
      <div class="h-line"></div>
      <p>This month goal is 45</p>
      <div class="list">
        <ul v-for="list in lists" :key="list.name">
          <li>
            <img
              src="../../../assets/icons8-cat-profile-48.png"
              width="20px"
              height="20px"
            />
          </li>
          <li>{{ list.name }}</li>
          <li>{{ list.days }}</li>
        </ul>
      </div>
      <p class="all-guests">SEE ALL GUESTS</p>
    </div>
  </div>
</template>

<script>
import BarChart from "vue-bar-chart";
export default {
  components: {
    BarChart,
  },
  data() {
    return {
      width: 250,
      height: 280,
      lists: [
        { name: "Fakhri Shokoohi", days: "2 days" },
        { name: "Linzell Bowman", days: "3 days" },
        { name: "Pin Jung-Eum", days: "5 days" },
        { name: "Shinohara Ryoma", days: "8 days" },
        { name: "Winny Rearie", days: "12 days" },
      ],
      options: [
        {
          title: "Apr 2018",
          value: 20,
          color: "#1971c2",
        },
        {
          title: "May 2018",
          value: 25,
          color: "#1971c2",
        },
        {
          title: "Jun 2018",
          value: 12,
          color: "#1971c2",
        },
        {
          title: "Jul 2018",
          value: 15,
          color: "#1971c2",
        },
        {
          title: "Aug 2018",
          value: 30,
          color: "#1971c2",
        },
        {
          title: "Sep 2018",
          value: 13,
          color: "#1971c2",
        },
        {
          title: "Oct 2018",
          value: 7,
          color: "#1971c2",
        },
      ],
    };
  },
};
</script>

<style scoped>
.satisfaction {
  border: 1px solid #ced4da;
  border-radius: 10px;
  width: 210px;
  height: 120px;
}

.heading {
  font-size: 16px;
  margin-left: 25px;
  margin-top: 10px;
}

.rate {
  font-weight: 100;
  display: flex;
  align-items: center;
  margin-left: 25px;
}
.rate img {
  margin-bottom: 10px;
  margin-right: 5px;
}

.rate p {
  color: #3a5e04;
  font-weight: 500;
  margin-top: 5px;
}

.emojis {
  display: flex;
  margin-left: 25px;
}

.emoji1,
.emoji2,
.emoji3 {
  display: flex;
  margin-right: 10px;
}

.emoji2 img {
  margin-top: -5px;
}

.emoji1 h6,
.emoji2 h6,
.emoji3 h6 {
  margin-left: 5px;
}

.bar-chart {
  border: 1px solid #ced4da;
  border-radius: 10px;
  width: 400px;
  height: 300px;
}

.barchart {
}

.grid-3-cols {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
  column-gap: 10px;
  margin-top: 30px;
}

.col2 {
  border: 1px solid #ced4da;
  border-radius: 10px;
  height: 340px;
  width: 250px;
}

.col2-heading {
  display: flex;
  justify-content: space-around;
  align-items: center;
  margin-top: 10px;
}
.booking {
  font-size: 16px;
}

.manage {
  font-size: 13px;
}

.col3 {
  border: 1px solid #ced4da;
  border-radius: 10px;
  width: 190px;
  margin-right: 5px;
}

.col3 h6 {
  margin-top: 10px;
  margin-left: 7px;
}

.col3 .rate {
  margin-left: 7px;
}

.h-line {
  border: 1px solid #3a5e04;
  margin-left: 7px;
  margin-right: 5px;
  width: 170px;
  height: 6px;
  border-radius: 4px;
  background-color: #1971c2;
  background-image: linear-gradient(to right, blue 50%, white 50%);
}

p {
  margin-left: 8px;
  margin-top: 8px;
}

.list {
  margin-left: -20px;
}

ul {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  row-gap: 1px;
}

li {
  list-style-type: none;
}

.tasks {
  border: 1px solid #ced4da;
  width: 210px;
  height: 210px;
  margin-top: 10px;
  border-radius: 10px;
}

.tasks-info {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-left: 15px;
  margin-top: -10px;
}

.room-info {
  line-height: 0.25;
}

hr {
  margin-left: 25px;
  margin-right: 25px;
  margin-top: -5px;
}

.tasks2-info {
  display: flex;
  justify-content: space-around;
  align-items: center;
  margin-left: 15px;
  margin-top: -10px;
}

.room2-info {
  line-height: 0.25;
}

.room2-info span {
  background-color: #d6336c;
  color: white;
  border-radius: 3px;
  padding: 1px;
  margin-left: 2px;
}

.all-tasks {
  margin-left: 20px;
}

.all-guests {
  margin-left: 15px;
}

.grid-cols-2 {
  display: grid;
  grid-template-columns: 2fr 1fr;
  column-gap: 10px;
  margin-top: 6px;
}

.calendar {
  border: 1px solid #ced4da;
  width: 475px;
  height: 255px;
  border-radius: 10px;
}

.cal-header {
  margin-left: 30px;
  margin-top: 20px;
  font-size: 16px;
}

.activity-log {
  border: 1px solid #ced4da;
  border-radius: 10px;
  margin-right: 5px;
}

.activity-log hr {
  margin-bottom: 20px;
}

.activity {
  font-size: 16px;
  margin-left: 15px;
}

.log {
  display: flex;
  justify-content: space-between;
  margin-left: 10px;
  margin-right: 5px;
}

.log p {
  margin-top: -10px;
  margin-bottom: -10px;
}

.room-details {
  margin-left: 15px;
  font-size: 13px;
}

.room-details span {
  color: red;
}

table {
  border: 1px solid #ced4da;
  width: 200px;
  height: 180px;
  border-spacing: 0;
  border-collapse: separate;
  border-radius: 10px;
  margin-left: 10px;
  overflow: hidden;
}

tr,
td {
  border: 1px solid #ced4da;
  text-align: center;
}

.september {
  display: grid;
  grid-template-columns: 1fr 1fr;
}

.sept {
  margin-top: -30px;
  margin-left: 150px;
  margin-bottom: 5px;
}

.info {
  display: flex;
  justify-content: space-between;
  margin-right: 6px;
  margin-top: -30px;
}

.rooms-data {
  border: 1px solid #ced4da;
  width: 230px;
  height: 50px;
  border-radius: 10px;
  margin-top: -10px;
}

.rooms-data1 {
  border: 1px solid #ced4da;
  width: 230px;
  height: 50px;
  border-radius: 10px;
  margin-top: 6px;
}

.rooms-villa {
  border: 1px solid #ced4da;
  width: 230px;
  height: 50px;
  border-radius: 10px;
  margin-top: 6px;
}

.profiles {
  display: flex;
  justify-content: space-between;
  margin-top: -12px;
  margin-left: 10px;
}

.profiles p {
  margin-right: 10px;
  margin-top: -1px;
}

.villa-profiles {
  display: flex;
  justify-content: space-between;
  margin-top: -15px;
  margin-left: 5px;
}

.villa-profiles p {
  margin-right: 5px;
  margin-top: -1px;
}
</style>
