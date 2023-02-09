<template>
  <div class="container">
    <div class="dots">
      <img src="../../assets/red.png" alt="red" width="15px" height="15px" />
      <img
        src="../../assets/yellow.png"
        alt="yellow"
        width="15px"
        height="15px"
      />
      <img
        src="../../assets/green.png"
        alt="green"
        width="15px"
        height="15px"
      />
    </div>
    <div>
      <img
        src="../../assets/diamond1.png"
        alt="diamond"
        width="40px"
        height="40px"
        class="diamond"
      />
    </div>
    <div class="icons">
      <img src="../../assets/clock.png" width="25px" height="25px" />
      <img src="../../assets/home.png" width="25px" height="25px" />
      <img src="../../assets/people.png" width="25px" height="25px" />
      <img src="../../assets/chat.png" width="25px" height="25px" />
      <img src="../../assets/inbox.png" width="25px" height="25px" />
      <img src="../../assets/trash.png" width="25px" height="25px" />
    </div>
    <div class="profile-icons">
      <img
        src="../../assets/network.png"
        width="20px"
        height="20px"
        class="network"
      />
      <img
        src="../../assets/icons8-cat-profile-48.png"
        alt="profile"
        width="30px"
        height="30px"
      />
    </div>
  </div>
</template>

<script></script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
}

.dots {
  display: flex;
  margin-bottom: 10px;
  margin-top: 10px;
}
.diamond {
  margin-bottom: 50px;
}

.icons {
  margin-bottom: 20px;
}

.icons img {
  margin-bottom: 30px;
  font-weight: 100;
}

.profile-icons img {
  margin-top: 110px;
}

.network {
  margin-bottom: -80px;
}
</style>
