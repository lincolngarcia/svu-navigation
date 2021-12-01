<template>
  <!--
        NOTES::
        INCREASE SPACING ON LEFT SIDE OF CARD ICONS ON LARGE DISPLAYS
        1. Triple Columns appear t 1408px, and at 417px, white space start to show
        2. SCRIPT NOT TESTED
        3. LINKS CANNOT BE ADDED UNTIL LINKS ARE GIVEN
        5. SOCIAL MEDIA ICONS NEED TO BE UPDATED WITH NEW THEME
  -->
  <div id="nav.encapsulation" style="max-width: 1600px; margin: 0 auto;">
    <div id="nav" class="nav flex">
      <div id="nav.left" class="left">
        <div id="nav.left.header" class="flex leftheader">
          <img
            src="~/assets/svg/Southern Virginia Logo.svg"
            class="mainLogo relative"
          />
          <div id="nav.content.header.contactUs" class="flex topAlign">
            <a class="standardText contactUs" href=""
              >Contact Us <!-- add Apply, Visit, Contact Us -->
              <img class="ContactUsImage" src="~/assets/svg/Arrow+Circle.svg"
            /></a>
            <a id="nav.content.header.whiteX" class="standardText whiteX">
              <img
                class="whiteX"
                src="~/assets/svg/Close Menu Icon White.svg"
              />
            </a>
          </div>
        </div>
        <div id="nav.left.content" class="left-padding">
          <ul class="leftContentItems">
            <li><a href="https://svu.edu/about/">Mission</a></li>
            <li><a href="https://svu.edu/academics/">Academics</a></li>
            <li><a href="">Our Virginia Home</a></li> <!-- anchor to Other attractions on locations page, change heading to our virginia home -->
            <li><a href="https://svu.edu/about/launchpad/">LaunchPad Initiative</a></li>
            <!--<li><a href="">Popular Programs</a></li>-->
            <li><a href="https://svu.edu/admissions/tuition-and-payments/">Tuition & Aid</a></li>
            <li><a href="https://svu.edu/application/">Apply</a></li>
          </ul>
          <br />
          <br />
          <div id="nav.content.bottomRow" class="flex">
            <img src="~/assets/svg/Social Media Icons.svg" />
            <!-- insert updated social media icons here -->
          </div>
          <br />
          <p class="standardText">News</p>
          <p class="standardText">Calendar & Events</p>
          <br />
          <div id="nav.left.footer" class="bottomArrow">
            <img src="~/assets/svg/arrow-down.svg" />
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
            src="~/assets/svg/Close Menu icon Red.svg"
          />
        </div>
        <div id="nav.right.content" class="relative wrap rightContentItems">
          <div id="academics">
            <h4>Academics</h4> <!-- create dynmaic loading -->
            <ul>
              <li><a href="https://svu.edu/faculty/">Our Faculty</a></li>
              <li><a href="https://svu.edu/academics/">Our Learning Model</a></li>
              <li><a href="https://svu.edu/academics/#programs">Programs & Degrees</a></li>
              <li><a href="https://svu.edu/academics/honors-program/">Honors Program</a></li>
              <li><a href="https://catalog.svu.edu">Catalog</a></li>
            </ul>
          </div>
          <div id="church_faith">
            <h4>Church & Faith</h4>
            <ul>
              <!--<li><a href="">Church Alignment *</a></li>-->
              <li><a href="https://svu.edu/campus-life/ysa-wards/">YSA Stake & Wards</a></li>
              <li><a href="https://www.southernvirginiainstitute.com/">Institute of Religion</a></li>
              <li><a href="https://svu.edu/campus-life/missionaries/">Missionaries</a></li>
            </ul>
          </div>
          <div id="giving">
            <h4>Giving</h4>
            <ul>
              <li><a href="https://secure.svu.edu/donate/">Make a Donation</a></li>
              <li><a href="">Why Give? *</a></li>
              <li><a href="https://svu.edu/giving/#priorities">Ways to Give</a></li>
              <!--<li><a href="">Capital Projects *</a></li>-->
            </ul>
          </div>
          <div id="admissions">
            <h4>Admissions</h4>
            <ul>
              <li><a href="https://svu.edu/application/">Apply Now</a></li>
              <li><a href="https://svu.edu/admissions/contact/">Admissions Team</a></li>
              <li><a href="https://svu.edu/admissions/#apply">How to Apply</a></li>
              <li><a href="https://svu.edu/admissions/enrollment/">How to Enroll</a></li>
              <li><a href="https://svu.edu/admissions/visit/">Visit Campus</a></li>
            </ul>
          </div>
          <div id="campus_life">
            <h4>Campus Life</h4>
            <ul>
              <li><a href="">Our Campus *</a></li>
              <li><a href="https://svu.edu/campus-life/code-of-honor/">Code of Conduct</a></li>
              <li><a href="https://svu.edu/campus-life/student-success/">Student Services</a></li>
              <li><a href="https://svu.edu/campus-life/dining/">Food Services</a></li>
              <li><a href="https://svu.edu/campus-life/housing/">University Housing</a></li>
              <li><a href="https://svu.edu/about/location/">Explore Virginia</a></li>
            </ul>
          </div>
          <div id="shop">
            <h4>Shop</h4>
            <ul>
              <li><a href="https://gear.svu.edu">Shop Athletics Gear</a></li>
              <li><a href="https://svu.textbookx.com/institutional/index.php">Online Bookstore</a></li>
              <li><a href="https://svu.merchorders.com/">Online Giftshop</a></li>
              <li><a href="https://photos.svu.edu/">Photo Store</a></li>
            </ul>
          </div>
          <div id="tuition_aid">
            <h4>Tuition & Aid</h4>
            <ul>
              <li><a href="https://svu.edu/admissions/financial-services/">Financial Aid Team</a></li>
              <li><a href="https://svu.edu/admissions/scholarships-and-aid/">Scholarships & Aid</a></li>
              <li><a href="https://svu.edu/admissions/tuition-and-payments/">Tution & Payments</a></li>
              <li><a href="https://svu.edu/admissions/scholarships-and-aid/">About the FAFSA</a></li> <!-- duplicate -->
            </ul>
          </div>
          <div id="popular_programs">
            <h4>Popular Programs</h4> <!-- irregularities in domain names should be addressed in new website -->
            <ul>
              <li><a href="https://art.svu.edu/">Art + Design</a></li>
              <li><a href="https://svu.edu/campus-life/athletics/">Athletics</a></li> <!-- mulitiple athletics pages -->
              <li><a href="https://esports.svu.edu/">Esports</a></li>
              <li><a href="https://music.svu.edu/">Music</a></li>
              <li><a href="https://svu.edu/campus-life/marching-band/">Marching Band</a></li>
              <!--<li><a href="">Student Leadership *</a></li>-->
              <li><a href="https://svu.edu/campus-life/theatre/">Theatre</a></li>
              <li><a href="https://svu.edu/academics/programs/pre-law/">Pre-Law</a></li>
              <li><a href="https://catalog.svu.edu/concentrations/pre-medical/">Pre-Med</a></li> <!-- irregularity from pre law  -->
            </ul>
          </div>
          <div id="tools">
            <h4>Tools</h4>
            <ul>
              <li><a href="https://svu.edu/about/alumni/">Alumni</a></li>
              <li><a href="https://svu.edu/canvas/">Canvas</a></li>
              <li><a href="https://calendar.svu.edu/">Calendars</a></li>
              <li><a href="https://catalog.svu.edu/">Catalog</a></li>
              <li><a href="https://svu.edu/directory/">Directory</a></li>
              <li><a href="https://svu.edu/employment/">Employment</a></li>
              <!--<li><a href="">Knight App *</a></li>-->
              <li><a href="https://my.svu.edu/ics">my<strong>svu</strong></a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div id="left.background" style="z-index: -1;" class="leftBackground"></div>
  </div>
</template>

<script>
export default {
  methods: {
    return: null
  }
};
</script>
<style>
*,
*::before,
*::after {
  margin: 0;
  box-sizing: border-box;
}
ul {
  padding: 0;
}
li {
  list-style: none;
}
a {
  text-decoration: none;
}
.nav {
  width: 100%;
}
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
  min-width: 50%;
  background-color: #9e1b32;
}
.left-padding {
  padding: 5% 20%;
}
.right {
  width: 50%;
}
.leftheader {
  justify-content: space-between;
  padding: 10% 5% 5% 5%;
}
.leftBackground {
  width: 50%;
  height: 100%;
  position: absolute;
  background-color: #9e1b32;
  top: 0;
  left: 0;
}
.rightheader {
  width: 100%;
  padding: 10% 5% 5% 5%;
  justify-content: flex-end;
  min-height: 4rem;
  max-width: 799px;
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
  margin-bottom: 10%;
}

ul.leftContentItems > li {
  white-space: nowrap;
  margin-bottom: 0.8rem;
}
ul.leftContentItems > li > a {
  font-family: "Avenir Next";
  color: white;
  font-weight: bold;
  font-size: 36px;
  font-weight: 600;
}
.rightContentItems {
  display: grid;
  grid-template-columns: .3333fr .3333fr .3333fr;
  gap: 20px 44px;
  padding: 10% 5% 5% 5%;
}
div.rightContentItems > div > h4 {
  color: #9e1b32;
  font-family: "Avenir Next";
  font-size: 18px;
  font-weight: 400;
  white-space: nowrap;
}
div.rightContentItems > div,
div.rightContentItems > div > ul > li > a {
  color: #707070;
  font-family: "Avenir Next";
  font-size: 16px;
  white-space: nowrap;
  align-items: start;
}

/* div.rightContentItems > div {
  padding: 16px;
} */

div.socialCircles {
  background-color: #fff;
  height: 18px;
  width: 18px;
}

@media screen and (max-width: 900px) {
  div.nav {
    display: block;
  }
  div.right {
    width: 100%;
  }
  div.left,
  .leftheader {
    width: 100%;
  }
  .leftBackground {
    display: none;
  }
  .rightheader,
  .contactUs {
    display: none;
  }
  .whiteX,
  .bottomArrow {
    display: flex;
  }

  ul.leftContentItems > li > a {
    font-size: 32px;
  }
}
@media screen and (max-width: 450px) {
  #academics {
    order: 1;
  }

  #campus_life {
    order: 2;
  }

  #admissions {
    order: 3;
  }

  #tuition_aid {
    order: 4;
  }

  #magnets {
    order: 5;
  }

  #church_faith {
    order: 6;
  }

  #giving {
    order: 7;
  }

  #tools {
    order: 8;
  }

  #shop {
    order: 10;
  }

  .rightContentItems {
    display: grid;
    grid-template-columns: 0.5fr 0.5fr;
    gap: 28px 16px;
    padding: 78px 28px 28px 28px;
  }

  div.rightContentItems > div,
  div.rightContentItems > div > ul > li > a {
    min-width: 0;
  }

  .left-padding {
    padding: 5% 10%;
  }
}
</style>
