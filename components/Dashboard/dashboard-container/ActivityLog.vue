<template>
  <div class="grid-cols-2">
    <div class="calendar">
      <p class="cal-header">Calendar</p>
      <p class="sept">September</p>

      <div class="september">
        <table>
          <tr>
            <td :style="{ 'font-weight': 100 }">27</td>
            <td :style="{ 'font-weight': 100 }">28</td>
            <td :style="{ 'font-weight': 100 }">29</td>
            <td :style="{ 'font-weight': 100 }">30</td>
            <td :style="{ 'font-weight': 100 }">31</td>
            <td>1</td>
            <td>2</td>
          </tr>
          <tr>
            <td>3</td>
            <td>4</td>
            <td>5</td>
            <td>6</td>
            <td>7</td>
            <td :style="{ 'background-color': 'black', color: 'white' }">8</td>
            <td>9</td>
          </tr>
          <tr>
            <td>10</td>
            <td>11</td>
            <td>12</td>
            <td>13</td>
            <td>14</td>
            <td>15</td>
            <td>16</td>
          </tr>
          <tr>
            <td>17</td>
            <td>18</td>
            <td>19</td>
            <td>20</td>
            <td>21</td>
            <td>22</td>
            <td>23</td>
          </tr>
          <tr>
            <td>24</td>
            <td>25</td>
            <td>26</td>
            <td>27</td>
            <td>28</td>
            <td>29</td>
            <td>30</td>
          </tr>
        </table>
        <div class="roomdata">
          <div class="info">
            <p>September 8</p>
            <p>3 rooms occupied</p>
          </div>

          <div class="rooms-data">
            <p>Room 103</p>
            <div>
              <div class="profiles">
                <div class="images">
                  <img
                    src="../../../assets/icons8-cat-profile-48.png"
                    width="15px"
                    height="15px"
                  />
                  <img
                    src="../../../assets/icons8-cat-profile-48.png"
                    width="15px"
                    height="15px"
                  />
                  <img
                    src="../../../assets/icons8-cat-profile-48.png"
                    width="15px"
                    height="15px"
                  />
                </div>
                <p>3 guests</p>
                <p>Sept 4 -- Sept 12</p>
              </div>
            </div>
          </div>
          <div class="rooms-data1">
            <p>Room 203</p>
            <div>
              <div class="profiles">
                <div class="images">
                  <img
                    src="../../../assets/icons8-cat-profile-48.png"
                    width="15px"
                    height="15px"
                  />
                  <img
                    src="../../../assets/icons8-cat-profile-48.png"
                    width="15px"
                    height="15px"
                  />
                </div>
                <p>2 guests</p>
                <p>Sept 6 -- Sept 12</p>
              </div>
            </div>
          </div>
          <div class="rooms-villa">
            <p>Villa</p>
            <div>
              <div class="villa-profiles">
                <div class="images">
                  <img
                    src="../../../assets/icons8-cat-profile-48.png"
                    width="15px"
                    height="15px"
                  />
                  <img
                    src="../../../assets/icons8-cat-profile-48.png"
                    width="15px"
                    height="15px"
                  />
                  <img
                    src="../../../assets/icons8-cat-profile-48.png"
                    width="15px"
                    height="15px"
                  />
                  <img
                    src="../../../assets/icons8-cat-profile-48.png"
                    width="15px"
                    height="15px"
                  />
                </div>
                <p>4 guests</p>
                <p>Sept 4 -- Sept 12</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="activity-log">
      <p class="activity">Activity Log</p>
      <div>
        <div class="log">
          <p>Room 103</p>
          <p>2 min</p>
        </div>
        <p class="room-details">
          Guest <span>Maria Peterson</span> entered room
        </p>
        <hr />
      </div>
      <div>
        <div class="log">
          <p>Room 103</p>
          <p>12 min</p>
        </div>
        <p class="room-details">Housekeeping exited room</p>
        <hr />
      </div>
      <div>
        <div class="log">
          <p>Room 203</p>
          <p>24 min</p>
        </div>
        <p class="room-details">Guests checked out</p>
        <hr />
      </div>
    </div>
  </div>
</template>

<style scoped>
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
