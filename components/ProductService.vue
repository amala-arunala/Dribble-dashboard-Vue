<template>
  <div class="container">
    <div class="avatar">
      <hr class="first" />
      <img src="../assets/customer.png" width="80px" height="80px" />
      <hr class="second" />
    </div>
    <div class="service">
      <h5>UXDN</h5>
      <p>Product Design as a service</p>
      <button>
        <img
          src="../assets/mail.png"
          width="20px"
          height="20px"
          class="saturate"
        />Hire Us
      </button>
    </div>
  </div>
</template>

<style scoped>
.container {
  font-family: "Roboto", sans-serif;
  margin-bottom: 100px;
}

.avatar {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 60px;
}

.first {
  width: 550px;
  margin-right: 15px;
}

.second {
  width: 550px;
  margin-left: 15px;
}

.service {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-top: 30px;
}

button {
  border: none;
  background-color: #f06595;
  border-radius: 10px;
  color: white;
  padding: 8px 15px;
  font-weight: 500;
}

.saturate {
  margin-right: 5px;
  margin-top: -5px;
  filter: saturate(10);
}
</style>
