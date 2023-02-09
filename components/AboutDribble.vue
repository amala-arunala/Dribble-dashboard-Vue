<template>
  <div class="links-container">
    <div>
      <img src="../assets/logo.png" alt="logo" width="100px" height="100px" />
      <p>
        Dribbble is the world's leading community for creatives to share, grow,
        and get hired.
      </p>
      <div>
        <img
          src="../assets/icons8-dribbble-48.png"
          alt="dribble-ball"
          width="35px"
          height="30px"
        />
        <img src="../assets/twitter.png" alt="twitter" />
        <img src="../assets/fb.png" alt="facebook" />
        <img
          src="../assets/insta.png"
          alt="instagram"
          width="30px"
          height="30px"
        />
        <img src="../assets/pinterest.png" alt="pinterest" />
      </div>
    </div>
    <div>
      <div class="link-heading">For designers</div>
      <a href="#" class="link">Go Pro!</a><br />
      <a href="#" class="link">Explore design work</a><br />
      <a href="#" class="link">Design blog</a><br />
      <a href="#" class="link">Overtime podcast</a><br />
      <a href="#" class="link">Playoffs</a><br />
      <a href="#" class="link">Weekly Warm-Up</a><br />
      <a href="#" class="link">Refer a Friend</a><br />
      <a href="#" class="link">Code of conduct</a><br />
    </div>
    <div>
      <div class="link-heading">Hire designers</div>
      <a href="#">Post a job opening</a><br />
      <a href="#">Post a freelance project</a><br />
      <a href="#">Search for designers</a><br /><br />
      <div class="link-heading">Brands</div>
      <a href="#">Advertise with us</a><br />
    </div>
    <div>
      <div class="link-heading">Company</div>
      <a href="#">About</a><br />
      <a href="#">Careers</a><br />
      <a href="#">Support</a><br />
      <a href="#">Media kit</a><br />
      <a href="#">Testimonials</a><br />
      <a href="#">API</a><br />
      <a href="#">Terms of service</a><br />
      <a href="#">Privacy policy</a><br />
      <a href="#">Cookie policy</a><br />
    </div>
    <div>
      <div class="link-heading">Directories</div>
      <a href="#">Design jobs</a><br />
      <a href="#">Designers for hire</a><br />
      <a href="#">Freelance designers for hire</a><br />
      <a href="#">Tags</a><br />
      <a href="#">Places</a><br /><br />
      <div class="link-heading">Design assets</div>
      <a href="#">Dribbble Marketplace</a><br />
      <a href="#">Creative Market</a><br />
      <a href="#">Fontspring</a><br />
      <a href="#">Font Squirrel</a><br />
    </div>
    <div>
      <div class="link-heading">Design Resources</div>
      <a href="#">Freelancing</a><br />
      <a href="#">Design Hiring</a><br />
      <a href="#">Design Portfolio</a><br />
      <a href="#">Design Education</a><br />
      <a href="#">Creative Process</a><br />
      <a href="#">Design Industry Trends</a><br />
    </div>
  </div>
</template>

<script></script>

<style scoped>
.links-container {
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  margin: 50px;
}

.link-heading {
  font-weight: 500;
  font-size: 16px;
  margin-bottom: 10px;
}

.link {
  margin-bottom: 8px;
}

a {
  text-decoration: none;
  color: black;
  font-weight: 300;
  font-size: 14px;
  margin-bottom: 10px;
}
</style>
