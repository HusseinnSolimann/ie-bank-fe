<template>
  <div class="home-page">
    <div class="header">
      <h1>Welcome to the IE Bank</h1>
      <p>Empowering your Financial Future</p>
    </div>
    <div class="buttons">
      <button class="cta-button" @click="goToAccounts">Go to Accounts</button>
      <button class="cta-button" @click="goToSkull">Go to Skull</button>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    goToAccounts() {
      this.$router.push('/accounts');
    },
    goToSkull() {
      this.$router.push('/skull');
    }
  }
};
</script>

<style scoped>
.home-page {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
}

.header {
  text-align: center;
  margin-bottom: 20px;
}

.header h1 {
  font-size: 36px;
  color: #333;
}

.header p {
  font-size: 18px;
  color: #666;
}

.buttons {
  display: flex;
}

.cta-button {
  margin: 0 10px;
  padding: 10px 20px;
  font-size: 18px;
  background-color: #007BFF;
  color: #fff;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.cta-button:hover {
  background-color: #0056b3;
}
</style>

