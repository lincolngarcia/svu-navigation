<template>
  <div id="nav" class="flex absolute">
    <div id="left" class="container left" sytle="width:40%;">
      <div id="left content header" class="mg-sides-40_32">
        <div id="header" class="flex header mg-top-40">
          <img src="~/assets/png/Southern Virginia Logo.png" class="mainlogo" />
          <a class="header-footerText" href="/revised"
            >Contact Us
            <img
              style="display: inline; max-height: 20px;"
              src="~/assets/png/Arrow+Circle.png"
          /></a>
        </div>
      </div>
      <div id="content" class="majorListItems">
        <ul>
          <li>Mission</li>
          <li>Academics</li>
          <li>Our Virginia Home</li>
          <li>LaunchPad Initiative</li>
          <li>Popular Programs</li>
          <li>Tuition & Aid</li>
          <li>Apply</li>
        </ul>
      </div>
      <div id="left content footer" class="header-footerText footer">
        <img src="~/assets/png/Social Media Icons.png" />
        <br />
        <p>News</p>
        <p>Calendar & Events</p>
      </div>
    </div>
    <div id="right" class="container" sytle="width:60%;">
      <div
        id="content"
        class="mg-top-40 mg-sides-64_40"
        style="position: relative;"
      >
        <img
          onclick="navClose()"
          style="position: absolute; right: 0px; top: 0px; max-height:16px;"
          src="~/assets/png/Close Menu Icon.png"
        />
        <div id="row1" class="flex">
          <div id="Academics" class="row-item">
          <h4>Academics</h4>
          <ul class='graytext'>
            <li>Our Faculty</li>
            <li>Our Learning Model</li>
            <li>Programs & Degrees</li>
            <li>Honors Program</li>
            <li>Catalog</li>
          </ul>
        </div>
          <div id="Church & Faith" class="row-item">
            <h4>Church & Faith</h4>
            <ul class="graytext">
              <li>Church Alignment</li>
              <li>YSA Stake & Wards</li>
              <li>Institute of Religion</li>
              <li>Missionaries</li>
            </ul>
          </div>
          <div id="Giving" class="row-item">
            <h4>Giving</h4>
            <ul class="graytext">
              <li>Make a Donation</li>
              <li>Why Give?</li>
              <li>Ways to Give</li>
              <li>Capital Projects</li>
            </ul>
          </div>
        </div>
        <div id="row2" class="flex">
          <div id="Admissions" class="row-item">
            <h4>Admissions</h4>
            <ul class="graytext">
              <li>Apply Now</li>
              <li>Admissions Team</li>
              <li>How to Apply</li>
              <li>How to Enroll</li>
              <li>Visit Campus</li>
            </ul>
          </div>
          <div id="Campus Life" class="row-item">
            <h4>Campus Life</h4>
            <ul class="graytext">
              <li>Our Campus</li>
              <li>Code of Conduct</li>
              <li>Student Services</li>
              <li>Food Services</li>
              <li>University Housing</li>
              <li>Explore Virginia</li>
            </ul>
          </div>
          <div id="Shop" class="row-item">
            <h4>Shop</h4>
            <ul class="graytext">
              <li>Shop Athletics Gear</li>
              <li>Online Bookstore</li>
              <li>Online Giftshop</li>
              <li>Photo Store</li>
            </ul>
          </div>
        </div>
        <div id="row3" class="flex">
          <div id="Tuition & Aid" class="row-item">
            <h4>Tuition & Aid</h4>
            <ul class="graytext">
              <li>Financial Aid Team</li>
              <li>Scholarships & Aid</li>
              <li>Tution & Payments</li>
              <li>About the FAFSA</li>
            </ul>
          </div>
          <div id="Popular Programs" class="row-item">
            <h4>Popular Programs</h4>
            <ul class="graytext">
              <li>Art + Design</li>
              <li>Athletics</li>
              <li>Esports</li>
              <li>Music</li>
              <li>Marching Band</li>
              <li>Student Leadership</li>
              <li>Theatre</li>
              <li>Pre-Law</li>
              <li>Pre-Med</li>
            </ul>
          </div>
          <div id="Tools" class="row-item">
            <h4>Tools</h4>
            <ul class="graytext">
              <li>Alumni</li>
              <li>Canvas</li>
              <li>Calendars</li>
              <li>Catalog</li>
              <li>Directory</li>
              <li>Employment</li>
              <li>Knight App</li>
              <li>my<strong>svu</strong></li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
function navClose() {
  console.log("yes");
  let id = null;
  const nav = document.getElementById("nav");
  var width = 100;
  clearInterval(id);
  id = setInterval(frame(), 10);
  function frame() {
    if (id == 0) {
      clearInterval(id);
    } else {
      width = width - 1;
      nav.style.maxWidth = width + "%";
    }
  }
}
</script>

<style scoped>
.mg-sides-64_40 {
  margin-left: 64px;
  margin-right: 40px;
}
.footer {
  margin-left: 15%;
  margin-top: 5%;
}
.mg-sides-40_32 {
  margin-left: 40px;
  margin-right: 32px;
}
.mg-top-40 {
  margin-top: 40px;
}
.header {
  width: 100%;
  justify-content: space-between;
}
.flex {
  display: flex;
}
h4 {
  color: #9e1b32;
  font-family: "Avenir Next";
  font-weight: 18px;
}
.graytext {
  color: #707070;
  font-family: "Avenir Next";
  font-size: 16px;
}
.left {
  background-color: #9e1b32;
}
.row-item {
  padding: 16px;
}
.majorListItems {
  margin-left: 15%;
  margin-top: 5%;
  color: white;
  font-weight: bold;
  font-size: 36px;
  font-weight: 600;
  font-family: "Avenir Next";
}
.mainlogo {
  max-width: 133px;
}
.header-footerText {
  color: white;
  font-weight: 600;
  font-family: "Avenir Next";
  font-size: 18px;
}
.absolute {
  position: absolute;
}
</style>
