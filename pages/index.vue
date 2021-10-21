<template>
 <!--
        NOTES::
        1. ADD EVENT LISTENER PREVENTS PAGE FROM LOADING
        2. SCRIPT NOT TESTED
        3. LINKS CANNOT BE ADDED UNTIL LINKS ARE GIVEN
        4. DIV WILL NOT TAKE UP FULL SCREEN
        5. SOCIAL MEDIA ICONS NEED TO BE UPDATED WITH NEW THEME
        6. WRAPPING DIV NEEDS TO WRAP ON ANYMORE THAN 3 ELEMENTS
        7. PAGE LINKS ARE KEPT FROM WRAPPING; GOOD IDEA OR NOT? SCRIPT-RIGHTCONTENTITEMS
        8. OPENING THE NAV SCRIPT DOES NOT EXIST
  -->
  <div id="nav" class="flex absolute">
    <div id="left" class="left">
      <div id="nav.left.header" class="flex header">
        <img src="~/assets/png/Southern Virginia Logo.png" class="mainLogo relative" />
        <a class="standardText" href=""
          >Contact Us <img class="contactUs" src="~/assets/png/Arrow+Circle.png"
        /></a>
      </div>
      <div id="nav.left.content" class="relative leftContentItems">
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
      <div id="nav.left.footer" class="standardText footer">
        <img src="~/assets/png/Social Media Icons.png" />
        <!-- <ol id="nav.left.footer.social_list" class='socialCircles'>
        <li>
          <a href="https://www.instagram.com/svuedu/" data-toggle="tooltip" title="" data-original-title="Instagram">
              <img src="/wp-content/uploads/instagram.png">
          </a>
        </li>
        <li>
          <a href="https://www.facebook.com/southernvirginia/" data-toggle="tooltip" title="" data-original-title="Facebook">
              <img src="/wp-content/uploads/facebook.png">
          </a>
        </li>
        <li>
          <a href="https://www.youtube.com/user/SouthernVirginiaUniv/" data-toggle="tooltip" title="" data-original-title="YouTube">
              <img src="/wp-content/uploads/youtube.png">
          </a>
        </li>
        <li>
          <a href="https://twitter.com/SVUedu/" data-toggle="tooltip" title="" data-original-title="Twitter">
              <img src="/wp-content/uploads/twitter.png">
          </a>
        </li>
        <li>
          <a href="https://www.linkedin.com/school/southern-virginia-university/" data-toggle="tooltip" title="" data-original-title="LinkedIn">
              <img src="/wp-content/uploads/linkedin.png">
          </a>
        </li>
      </ol> -->
        <br />
        <p>News</p>
        <p>Calendar & Events</p>
      </div>
    </div>
    <div id="nav.right" class="relative right">
      <img
        id='closeButton'
        class="absolute closeButton"
        src="~/assets/png/Close Menu icon.png"
      />
      <div id="nav.right.content" class="relative wrap rightContentItems">
        <div id="nav.right.content.academics">
          <h4>Academics</h4>
          <ul>
            <li>Our Faculty</li>
            <li>Our Learning Model</li>
            <li>Programs & Degrees</li>
            <li>Honors Program</li>
            <li>Catalog</li>
          </ul>
        </div>
        <div id="nav.right.content.church_&_faith">
            <h4>Church & Faith</h4>
            <ul>
              <li>Church Alignment</li>
              <li>YSA Stake & Wards</li>
              <li>Institute of Religion</li>
              <li>Missionaries</li>
            </ul>
          </div>
        <div id="nav.right.content.giving">
          <h4>Giving</h4>
          <ul>
            <li>Make a Donation</li>
            <li>Why Give?</li>
            <li>Ways to Give</li>
            <li>Capital Projects</li>
          </ul>
        </div>
        <div id="nav.right.content.admissions">
          <h4>Admissions</h4>
          <ul>
            <li>Apply Now</li>
            <li>Admissions Team</li>
            <li>How to Apply</li>
            <li>How to Enroll</li>
            <li>Visit Campus</li>
          </ul>
        </div>
        <div id="nav.right.content.campus_life">
          <h4>Campus Life</h4>
          <ul>
            <li>Our Campus</li>
            <li>Code of Conduct</li>
            <li>Student Services</li>
            <li>Food Services</li>
            <li>University Housing</li>
            <li>Explore Virginia</li>
          </ul>
        </div>
        <div id="nav.right.content.shop">
          <h4>Shop</h4>
          <ul>
            <li>Shop Athletics Gear</li>
            <li>Online Bookstore</li>
            <li>Online Giftshop</li>
            <li>Photo Store</li>
          </ul>
        </div>
        <div id="nav.right.content.tuition_&_aid">
          <h4>Tuition & Aid</h4>
          <ul>
            <li>Financial Aid Team</li>
            <li>Scholarships & Aid</li>
            <li>Tution & Payments</li>
            <li>About the FAFSA</li>
          </ul>
        </div>
        <div id="nav.right.content.popular_programs">
          <h4>Popular Programs</h4>
          <ul>
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
        <div id="nav.right.content.tools">
          <h4>Tools</h4>
          <ul>
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
</template>

<script>
export default {};
document.getElementById("closeButton").addEventListener("click",navClose);
//nav.addEventListener("click",navClose);
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
.flex {
  display: flex;
}
.absolute {
  display: absolute;
}
.relative {
  display: relative;
}
.wrap {
    display: flex;
    flex-wrap: wrap;
}
.left {
  background-color: #9e1b32;
  width: 40%;
}
.right {
  width: 60%;
  margin-top: 40px;
  margin-right: 64px;
  margin-left: 40px;
}
.header {
  justify-content: space-between;
  margin-top: 40px;
  margin-left: 40px;
  margin-right: 32px;
}
.footer {
    margin-left: 15%;
    margin-top: 5%;
}
.mainLogo {
  max-width: 133px;
  left: -8px;
  top: -8px;
}
.contactUs {
  display: inline;
  max-height: 20px;
}
.closeButton {
    right: 0px;
    top: 0px;
    max-height: 16px;
}
.standardText {
  color: white;
  font-weight: 600;
  font-family: "Avenir Next";
  font-size: 18px;
}
div.leftContentItems {
  color: white;
  font-weight: bold;
  font-size: 36px;
  font-weight: 600;
  font-family: "Avenir Next";
  margin-left: 15%;
  margin-top: 5%;
}
div.rightContentItems > div > h4 {
  color: #9e1b32;
  font-family: "Avenir Next";
  font-weight: 18px;
  white-space: nowrap;
}
div.rightContentItems > div> ul > li {
  color: #707070;
  font-family: "Avenir Next";
  font-size: 16px;
  white-space: nowrap;
}
div.rightContentItems > div {
    padding: 16px;
}
div.socialCircles {
    background-color: #fff;
    height: 18px;
    width: 18px;
    opacity: 0.7;
}
</style>