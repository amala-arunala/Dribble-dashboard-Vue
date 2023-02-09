<template>
  <div class="dashboard">
    <div class="overview">
      <h4>Dashboard</h4>
      <button class="overview-btn">
        Overview<img
          src="../../../assets/arrow.png"
          width="15px"
          height="15px"
          class="down-arrow"
        />
      </button>
    </div>
    <div>
      <button>
        <img
          src="../../../assets/person.png"
          width="20px"
          height="20px"
          class="person"
        />New Guest
      </button>
      <button>
        <img
          src="../../../assets/edit.png"
          width="15px"
          height="15px"
          class="edit"
        />New Reservation
      </button>
    </div>
  </div>
</template>

<script></script>

<style scoped>
.dashboard {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.overview {
  display: flex;
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
</style>
