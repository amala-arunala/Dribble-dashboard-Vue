<template>
  <div class="header">
    <div class="profile">
      <img
        src="../../assets/icons8-cat-profile-48.png"
        alt="profile"
        width="60px"
        height="60px"
        class="profile-img"
      />
      <div class="profile-desc">
        <h5>Hotel Dashboard</h5>
        <p>
          Alex Tsibulski for UXDN . Follow . <span class="hire">Hire Us</span>
        </p>
      </div>
    </div>
    <div class="btns">
      <button class="save-btn">Save</button>
      <button class="like-btn"><span>❤</span>Like</button>
    </div>
  </div>
</template>

<script></script>

<style scoped>
.header {
  display: flex;
  justify-content: space-around;
  align-items: center;
  margin: 30px;
  font-family: "Roboto", sans-serif;
}

.profile {
  display: flex;
  margin-left: 100px;
}

.profile-img {
  margin-right: 10px;
}

.profile-desc {
  padding-top: 10px;
  line-height: 0.75;
}

p {
  font-size: 16px;
}

.hire {
  color: #ff6b6b;
}

.btns {
  margin-right: 200px;
}

.save-btn {
  border: none;
  border-radius: 8px;
  margin-right: 10px;
  padding: 8px 12px;
  font-size: 16px;
  font-weight: 500;
}

.like-btn {
  border: none;
  border-radius: 8px;
  border-radius: 6px;
  padding: 8px 12px;
  background-color: #d6336c;
  color: white;
  font-size: 16px;
  font-weight: 500;
}

span {
  margin-right: 4px;
}
</style>
