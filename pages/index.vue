<template>
  <!--
        NOTES::
        2. SCRIPT NOT TESTED
        3. LINKS CANNOT BE ADDED UNTIL LINKS ARE GIVEN
        5. SOCIAL MEDIA ICONS NEED TO BE UPDATED WITH NEW THEME
        6. WRAPPING DIV NEEDS TO WRAP ON ANYMORE THAN 3 ELEMENTS
  -->
  <div id="nav" class="nav flex">
    <div id="nav.left" class="left">
      <div id="nav.left.header" class="flex leftheader">
        <img
          src="~/assets/png/Southern Virginia Logo.png"
          class="mainLogo relative"
        />
        <div id="nav.content.header.contactUs" class="flex topAlign">
          <a class="standardText contactUs" href=""
            >Contact Us
            <img class="ContactUsImage" src="~/assets/png/Arrow+Circle.png"
          /></a>
          <a id="nav.content.header.whiteX" class="standardText whiteX">
            <img
              class="whiteX"
              src="~/assets/png/Close Menu Icon -- white.png"
            />
          </a>
        </div>
      </div>
      <div id="nav.left.content" class="left-padding">
        <ul class="leftContentItems">
          <li><a href="">Mission</a></li>
          <li><a href="">Academics</a></li>
          <li><a href="">Our Virginia Home</a></li>
          <li><a href="">LaunchPad Initiative</a></li>
          <li><a href="">Popular Programs</a></li>
          <li><a href="">Tuition & Aid</a></li>
          <li><a href="">Apply</a></li>
        </ul>
        <br />
        <br />
        <div id="nav.content.bottomRow" class="flex">
          <img src="~/assets/png/Social Media Icons.png" />
          <!-- insert updated social media icons here -->
        </div>
        <br />
        <p class="standardText">News</p>
        <p class="standardText">Calendar & Events</p>
        <br />
        <div id="nav.left.footer" class="bottomArrow">
          <div id="nav.left.footer.left" class="">
            <img src="~/assets/png/line.png" style="right: -1px; transform: scaleX(-1);" />
          </div>
          <div id="nav.left.footer.right" class="">
            <img src="~/assets/png/line.png" style="left: -1px;" />
          </div>
        </div>
      </div>
    </div>
    <!--
      <ol id="nav.left.footer.social_list" class='socialCircles'>
        <li><a href=''>
          <a href="https://www.instagram.com/svuedu/" data-toggle="tooltip" title="" data-original-title="Instagram">
              <img src="/wp-content/uploads/instagram.png">
          </a>
        </a></li>
        <li><a href=''>
          <a href="https://www.facebook.com/southernvirginia/" data-toggle="tooltip" title="" data-original-title="Facebook">
              <img src="/wp-content/uploads/facebook.png">
          </a>
        </a></li>
        <li><a href=''>
          <a href="https://www.youtube.com/user/SouthernVirginiaUniv/" data-toggle="tooltip" title="" data-original-title="YouTube">
              <img src="/wp-content/uploads/youtube.png">
          </a>
        </a></li>
        <li><a href=''>
          <a href="https://twitter.com/SVUedu/" data-toggle="tooltip" title="" data-original-title="Twitter">
              <img src="/wp-content/uploads/twitter.png">
          </a>
        </a></li>
        <li><a href=''>
          <a href="https://www.linkedin.com/school/southern-virginia-university/" data-toggle="tooltip" title="" data-original-title="LinkedIn">
              <img src="/wp-content/uploads/linkedin.png">
          </a>
        </a></li>
      </ol>
-->
    <div id="nav.right" class="relative right">
      <div id="nav.right.header" class="flex rightheader">
        <img
          @click="navClose"
          id="closeButton"
          class="closeButton"
          src="~/assets/png/Close Menu icon -- red.png"
        />
      </div>
      <div id="nav.right.content" class="relative wrap rightContentItems">
        <div id="nav.right.content.academics">
          <h4>Academics</h4>
          <ul>
            <li><a href="">Our Faculty</a></li>
            <li><a href="">Our Learning Model</a></li>
            <li><a href="">Programs & Degrees</a></li>
            <li><a href="">Honors Program</a></li>
            <li><a href="">Catalog</a></li>
          </ul>
        </div>
        <div id="nav.right.content.church_&_faith">
          <h4>Church & Faith</h4>
          <ul>
            <li><a href="">Church Alignment</a></li>
            <li><a href="">YSA Stake & Wards</a></li>
            <li><a href="">Institute of Religion</a></li>
            <li><a href="">Missionaries</a></li>
          </ul>
        </div>
        <div id="nav.right.content.giving">
          <h4>Giving</h4>
          <ul>
            <li><a href="">Make a Donation</a></li>
            <li><a href="">Why Give?</a></li>
            <li><a href="">Ways to Give</a></li>
            <li><a href="">Capital Projects</a></li>
          </ul>
        </div>
        <div id="nav.right.content.admissions">
          <h4>Admissions</h4>
          <ul>
            <li><a href="">Apply Now</a></li>
            <li><a href="">Admissions Team</a></li>
            <li><a href="">How to Apply</a></li>
            <li><a href="">How to Enroll</a></li>
            <li><a href="">Visit Campus</a></li>
          </ul>
        </div>
        <div id="nav.right.content.campus_life">
          <h4>Campus Life</h4>
          <ul>
            <li><a href="">Our Campus</a></li>
            <li><a href="">Code of Conduct</a></li>
            <li><a href="">Student Services</a></li>
            <li><a href="">Food Services</a></li>
            <li><a href="">University Housing</a></li>
            <li><a href="">Explore Virginia</a></li>
          </ul>
        </div>
        <div id="nav.right.content.shop">
          <h4>Shop</h4>
          <ul>
            <li><a href="">Shop Athletics Gear</a></li>
            <li><a href="">Online Bookstore</a></li>
            <li><a href="">Online Giftshop</a></li>
            <li><a href="">Photo Store</a></li>
          </ul>
        </div>
        <div id="nav.right.content.tuition_&_aid">
          <h4>Tuition & Aid</h4>
          <ul>
            <li><a href="">Financial Aid Team</a></li>
            <li><a href="">Scholarships & Aid</a></li>
            <li><a href="">Tution & Payments</a></li>
            <li><a href="">About the FAFSA</a></li>
          </ul>
        </div>
        <div id="nav.right.content.popular_programs">
          <h4>Popular Programs</h4>
          <ul>
            <li><a href="">Art + Design</a></li>
            <li><a href="">Athletics</a></li>
            <li><a href="">Esports</a></li>
            <li><a href="">Music</a></li>
            <li><a href="">Marching Band</a></li>
            <li><a href="">Student Leadership</a></li>
            <li><a href="">Theatre</a></li>
            <li><a href="">Pre-Law</a></li>
            <li><a href="">Pre-Med</a></li>
          </ul>
        </div>
        <div id="nav.right.content.tools">
          <h4>Tools</h4>
          <ul>
            <li><a href="">Alumni</a></li>
            <li><a href="">Canvas</a></li>
            <li><a href="">Calendars</a></li>
            <li><a href="">Catalog</a></li>
            <li><a href="">Directory</a></li>
            <li><a href="">Employment</a></li>
            <li><a href="">Knight App</a></li>
            <li>
              <a href="">my<strong>svu</strong></a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    return: null
  }
};
</script>

<style scoped>
.flex {
  display: flex;
}
.bottomArrow {
  width: 100%;
  display: none;
  justify-content: center;
}
div.bottomArrow > div > img {
  max-height: 40px;
  position: relative;
}
.flex-end {
  justify-content: flex-end;
}
.relative {
  position: relative;
}
.wrap {
  display: flex;
  flex-wrap: wrap;
}
.left {
  background-color: #9e1b32;
  min-width: 50%;
}
.left-padding {
  padding-left: 20%;
  padding-right: 20%;
  padding-top: 25%;
  padding-bottom: 5%;
}
.right {
  width: 50%;
  margin-top: 30px;
  margin-right: 64px;
  margin-left: 40px;
}
.leftheader {
  width: 50%;
  position: absolute;
  justify-content: space-between;
  padding: 5%;
}
.rightheader {
  width: 100%;
  padding-top: 5%;
  justify-content: flex-end;
  min-height: 4rem;
}
.mainLogo {
  max-width: 133px;
  left: -8px;
  top: -8px;
}
.contactUs {
  display: flex;
  align-items: center;
  white-space: nowrap;
}
.whiteX {
  display: none;
}
.topAlign {
  flex-direction: column;
  justify-content: flex-start;
}
.ContactUsImage {
  margin-left: 0.5rem;
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
ul.leftContentItems > li {
  color: white;
  font-weight: bold;
  font-size: 36px;
  font-weight: 600;
  font-family: "Avenir Next";
  white-space: nowrap;
  margin-bottom: 0.8rem;
}
div.rightContentItems > div > h4 {
  color: #9e1b32;
  font-family: "Avenir Next";
  font-weight: 18px;
  white-space: nowrap;
}
div.rightContentItems > div {
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
}
@media screen and (max-width: 600px) {
  div.nav {
    display: block;
  }
  div.right {
    width: 100%;
  }
  div.left {
    width: 100%;
  }
  .leftheader {
    width: 100%;
  }
  .rightheader {
    display: none;
  }
  .contactUs {
    display: none;
  }
  .whiteX {
    display: block;
  }
  .bottomArrow {
    display: flex;
  }
}
</style>
