<template>
  <div class="container">
    <div class="inner-container">
      <div>
        <a href="#">Updates</a>
      </div>
      <div class="user">
        <p>Session 34 minutes</p>
        <p>User : Ann Tsilbulski</p>
      </div>
    </div>
    <DashboardHeader />
    <ManageBookings />
    <ActivityLog />
  </div>
</template>

<script>
import DashboardHeader from "../Dashboard/dashboard-container/DashboardHeader.vue";
import ManageBookings from "../Dashboard/dashboard-container/ManageBookings.vue";
import ActivityLog from "../Dashboard/dashboard-container/ActivityLog.vue";
export default {
  components: {
    DashboardHeader,
    ManageBookings,
    ActivityLog,
  },
  data() {
    return {};
  },
};
</script>

<style scoped>
.container {
  width: 700px;
  margin-left: 10px;
  font-size: 12px;
  font-family: "Roboto", sans-serif;
}

.inner-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

a {
  color: black;
}

.user {
  display: flex;
  align-items: center;
  margin-top: 15px;
}

.user p {
  margin-right: 10px;
}

button {
  border: none;
  border-radius: 40px;
  margin-right: 10px;
  padding: 3px 12px;
}

.overview-btn {
  padding: 0 15px;
  font-size: 14px;
  border-radius: 40px;
  padding: 3px 12px;
}

.dashboard {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.overview {
  display: flex;
}

.down-arrow {
  margin-left: 5px;
}
h4 {
  margin-right: 10px;
}

.person,
.edit {
  margin-right: 5px;
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
