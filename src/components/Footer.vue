<template>
  <div class="footer">
    <div class="grid-container-footer">
      <div class="grid-item1">
        <p class="item-header1">Enter your email address to get updates</p>
        <div class="item-details">
          <div class="details1">
            <input
              class="input"
              type="text"
              placeholder="Enter your email address"
            />
            <button class="details1-btn">Subscribe</button>
          </div>
        </div>
      </div>
      <div class="grid-item2">
        <p class="item-header2">enMasse</p>
        <div class="header2-list">
          <p>Home</p>
          <p>Products</p>
          <p>Categories</p>
          <p>About Us</p>
          <p>Make Request</p>
          <p>Become an Agent</p>
        </div>
      </div>
      <div class="grid-item2">
        <p class="item-header2">Terms</p>
        <div class="header2-list">
          <p>Terms of Use</p>
          <p>Privacy Policy</p>
          <img src="@/assets/social_icons.svg" />
        </div>
      </div>
    </div>
    <div>
      <p class="copyright">Copyright © 2020 enMasse. All Rights Reserved.</p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.grid-container-footer {
  display: grid;
  grid-template-columns: 1.5fr 0.5fr 1fr;
  justify-content: center;
  padding-top: 53px;
  box-sizing: border-box;
  border-bottom: 0.911729px solid #ffffff;
}

.grid-item1 {
  max-width: 259px;
  margin-left: 200px;
}
.grid-item1 .input {
  width: 100%;
  background: #ffffff;
  border: 1px solid #828282;
  box-sizing: border-box;
  border-radius: 4px;
  height: 45px;
  margin-bottom: 75px;
  /* Text */
  font-family: Roboto;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 19px;
  color: #bdbdbd;
}
.grid-item1 .details1-btn {
  width: 100%;
  height: 50px;
  background: #ffa010;
  border: 1px solid #ffa010;
  border-radius: 4px;
}
.grid-item2 {
  margin: 0 0 70px;
}
.item-header1 {
  font-family: Mulish;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 20px;
  max-width: 259px;
  color: #ffffff;
  margin-bottom: 50px;
}
.item-header2 {
  font-family: Raleway;
  font-style: normal;
  font-weight: bold;
  font-size: 18px;
  line-height: 21px;
  color: #ffffff;
}
.header2-list {
  font-family: Mulish;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 20px;
  color: #ffffff;
}
.footer {
  background-color: #2e9eb6;
  margin-top: 73px;
}
.copyright {
  font-family: Mulish;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 20px;
  color: #ffffff;
  text-align: center;
  margin: 20px 0 21px 0;
}
</style>
