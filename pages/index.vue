<template>
  <nav id="nav.encapsulation" style="max-width: 1600px; margin: 0 auto;">
    <div id="nav" class="nav flex">
      <div id="nav.left" class="left">
        <div id="nav.left.header" class="flex leftheader">
          <img
            src="~/assets/svg/Southern Virginia Logo.svg"
            class="mainLogo relative"
          />
          <div id="nav.content.header.contactUs" class="flex topAlign">
            <div class="flex">
              <a class="standardText topalignChild">Apply</a>
              <a class="standardText topalignChild">Visit</a>
              <div class='topalignChild'>
                <a class="standardText contactUs" href=""
                  >Contact Us
                  <img
                    class="ContactUsImage"
                    src="~/assets/svg/Arrow+Circle.svg"
                /></a>
                <a id="nav.content.header.whiteX" class="standardText whiteX">
                  <img
                    class="whiteX"
                    src="~/assets/svg/Close Menu Icon White.svg"
                  />
                </a>
              </div>
            </div>
          </div>
        </div>
        <div id="nav.left.content" class="left-padding">
          <ul class="leftContentItems">
            <li><a href="https://svu.edu/about/">Mission</a></li>
            <li><a href="https://svu.edu/academics/">Academics</a></li>
            <li><a href="https://svu.edu/about/location/#our_virginia_home">Our Virginia Home</a></li>
            <!-- anchor to Other attractions on locations page, change heading to our virginia home DONE-->
            <li>
              <a href="https://svu.edu/about/launchpad/"
                >LaunchPad Initiative</a
              >
            </li>
            <!--<li><a href="">Popular Programs</a></li>-->
            <li>
              <a href="https://svu.edu/admissions/tuition-and-payments/"
                >Tuition &amp; Aid</a
              >
            </li>
            <li><a href="https://svu.edu/application/">Apply</a></li>
          </ul>
          <br />
          <br />
          <div id="nav.content.bottomRow" class="flex">
            <!-- SOCIAL MEDIA ICONS -->
            <ul id="nav.left.footer.social_list" class="socialCircles">
              <li>
                <a
                  class="socialIcon"
                  href="https://www.facebook.com/southernvirginia/"
                  data-toggle="tooltip"
                  title=""
                  data-original-title="Facebook"
                >
                  <svg
                    class="social-svg"
                    x="0px"
                    y="0px"
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 29.02 29"
                  >
                    <defs>
                      <style>
                        .cls-1 {
                          fill: #ffffff;
                        }
                      </style>
                    </defs>
                    <g id="Layer_2" data-name="Layer 2">
                      <g id="Layer_1-2" data-name="Layer 1">
                        <path
                          class="cls-1"
                          d="M14.51,0a14.51,14.51,0,0,0-4.45,28.32V17.76H7.31v-4h2.75V11.12c0-1.18,0-3,.88-4.12a4.9,4.9,0,0,1,4.27-2,17.4,17.4,0,0,1,4.92.49l-.69,4.07a9.24,9.24,0,0,0-2.21-.33c-1.07,0-2,.38-2,1.45v3.1h4.38l-.31,4H15.21V29a14.51,14.51,0,0,0-.7-29Z"
                        />
                      </g>
                    </g>
                  </svg>
                </a>
              </li>
              <li>
                <a
                  class="socialIcon"
                  href="https://www.instagram.com/svuedu/"
                  data-toggle="tooltip"
                  title=""
                  data-original-title="Instagram"
                >
                  <svg
                    class="social-svg"
                    x="0px"
                    y="0px"
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 503.84 503.84"
                  >
                    <defs>
                      <style>
                        .cls-1 {
                          fill: #ffffff;
                        }
                      </style>
                    </defs>
                    <g id="Layer_2" data-name="Layer 2">
                      <g id="Logo">
                        <path
                          class="cls-1"
                          d="M251.92,45.39c67.27,0,75.23.26,101.8,1.47,24.56,1.12,37.9,5.22,46.78,8.67a78,78,0,0,1,29,18.85,78,78,0,0,1,18.85,29c3.45,8.88,7.55,22.22,8.67,46.78,1.21,26.57,1.47,34.53,1.47,101.8s-.26,75.23-1.47,101.8c-1.12,24.56-5.22,37.9-8.67,46.78a83.51,83.51,0,0,1-47.81,47.81c-8.88,3.45-22.22,7.55-46.78,8.67-26.56,1.21-34.53,1.47-101.8,1.47s-75.24-.26-101.8-1.47c-24.56-1.12-37.9-5.22-46.78-8.67a78,78,0,0,1-29-18.85,78,78,0,0,1-18.85-29c-3.45-8.88-7.55-22.22-8.67-46.78-1.21-26.57-1.47-34.53-1.47-101.8s.26-75.23,1.47-101.8c1.12-24.56,5.22-37.9,8.67-46.78a78,78,0,0,1,18.85-29,78,78,0,0,1,29-18.85c8.88-3.45,22.22-7.55,46.78-8.67,26.57-1.21,34.53-1.47,101.8-1.47m0-45.39c-68.42,0-77,.29-103.87,1.52S102.93,7,86.9,13.23A123.52,123.52,0,0,0,42.28,42.28a123.52,123.52,0,0,0-29,44.62C7,102.93,2.74,121.24,1.52,148.05S0,183.5,0,251.92s.29,77,1.52,103.87S7,400.91,13.23,416.94a123.52,123.52,0,0,0,29.05,44.62A123.68,123.68,0,0,0,86.9,490.62c16,6.22,34.34,10.48,61.15,11.71s35.45,1.51,103.87,1.51,77-.29,103.87-1.51,45.12-5.49,61.15-11.71a128.85,128.85,0,0,0,73.68-73.68c6.22-16,10.48-34.34,11.71-61.15s1.51-35.45,1.51-103.87-.29-77-1.51-103.87-5.49-45.12-11.71-61.15a123.68,123.68,0,0,0-29.06-44.62,123.52,123.52,0,0,0-44.62-29C400.91,7,382.6,2.74,355.79,1.52S320.34,0,251.92,0Z"
                        />
                        <path
                          class="cls-1"
                          d="M251.92,122.56A129.37,129.37,0,1,0,381.29,251.92,129.35,129.35,0,0,0,251.92,122.56Zm0,213.33a84,84,0,1,1,84-84A84,84,0,0,1,251.92,335.89Z"
                        />
                        <circle
                          class="cls-1"
                          cx="386.4"
                          cy="117.44"
                          r="30.23"
                        />
                      </g>
                    </g>
                  </svg>
                </a>
              </li>
              <li>
                <a
                  class="socialIcon"
                  href="https://www.youtube.com/user/SouthernVirginiaUniv/"
                  data-toggle="tooltip"
                  title=""
                  data-original-title="YouTube"
                >
                  <svg
                    class="social-svg"
                    x="0px"
                    y="0px"
                    id="Layer_1"
                    data-name="Layer 1"
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 192 192"
                  >
                    <defs>
                      <style>
                        .cls-1 {
                          fill: #ffffff;
                        }
                      </style>
                    </defs>
                    <path
                      class="cls-1"
                      d="M180.32,53.36A22.12,22.12,0,0,0,164.76,37.7C151,34,96,34,96,34s-55,0-68.76,3.7A22.12,22.12,0,0,0,11.68,53.36C8,67.18,8,96,8,96s0,28.82,3.68,42.64A22.12,22.12,0,0,0,27.24,154.3C41,158,96,158,96,158s55,0,68.76-3.7a22.12,22.12,0,0,0,15.56-15.66C184,124.82,184,96,184,96S184,67.18,180.32,53.36ZM78,122.17V69.83L124,96Z"
                    />
                  </svg>
                </a>
              </li>
              <li>
                <a
                  class="socialIcon"
                  href="https://twitter.com/SVUedu/"
                  data-toggle="tooltip"
                  title=""
                  data-original-title="Twitter"
                >
                  <svg
                    class="social-svg"
                    x="0px"
                    y="0px"
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 400 400"
                  >
                    <defs>
                      <style>
                        .cls-1 {
                          fill: #ffffff;
                        }
                        .cls-2 {
                          fill: none;
                        }
                      </style>
                    </defs>
                    <g id="Layer_2" data-name="Layer 2">
                      <g id="Logo_FIXED" data-name="Logo — FIXED">
                        <rect
                          style="fill:none;"
                          class="cls-1"
                          width="400"
                          height="400"
                        />
                        <path
                          style="fill:white;"
                          class="cls-2"
                          d="M153.62,301.59c94.35,0,145.94-78.16,145.94-145.94q0-3.33-.15-6.63A104.36,104.36,0,0,0,325,122.47a102.42,102.42,0,0,1-29.46,8.07,51.52,51.52,0,0,0,22.56-28.37,102.91,102.91,0,0,1-32.57,12.45,51.34,51.34,0,0,0-87.41,46.77A145.62,145.62,0,0,1,92.4,107.81a51.31,51.31,0,0,0,15.88,68.47,50.87,50.87,0,0,1-23.23-6.42c0,.22,0,.43,0,.66a51.31,51.31,0,0,0,41.15,50.28,51.42,51.42,0,0,1-23.17.88,51.34,51.34,0,0,0,47.92,35.62,102.91,102.91,0,0,1-63.7,22A105.19,105.19,0,0,1,75,278.55a145.17,145.17,0,0,0,78.62,23"
                        />
                      </g>
                    </g>
                  </svg>
                </a>
              </li>
              <li>
                <a
                  class="socialIcon"
                  href="https://www.linkedin.com/school/southern-virginia-university/"
                  data-toggle="tooltip"
                  title=""
                  data-original-title="LinkedIn"
                >
                  <svg
                    class="social-svg"
                    x="0px"
                    y="0px"
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 94.39 94.39"
                  >
                    <defs>
                      <style>
                        .cls-1 {
                          fill: white;
                        }
                      </style>
                    </defs>
                    <g id="Layer_2" data-name="Layer 2">
                      <g id="Layer_1-2" data-name="Layer 1">
                        <path
                          class="cls-1"
                          d="M87.4,0H7A6.89,6.89,0,0,0,0,6.8V87.58a6.9,6.9,0,0,0,7,6.81H87.4a6.92,6.92,0,0,0,7-6.81V6.8A6.91,6.91,0,0,0,87.4,0ZM28,80.43H14v-45H28Zm-7-51.2a8.12,8.12,0,1,1,8.11-8.12A8.12,8.12,0,0,1,21,29.23Zm59.43,51.2h-14V58.52c0-5.22-.1-11.94-7.27-11.94s-8.41,5.69-8.41,11.57V80.43h-14v-45H50.2v6.15h.19c1.87-3.54,6.44-7.27,13.25-7.27,14.17,0,16.79,9.33,16.79,21.45Z"
                        />
                      </g>
                    </g>
                  </svg>
                </a>
              </li>
            </ul>
          </div>
          <br />
          <p class="standardText">News</p>
          <p class="standardText">Calendar &amp;amp; Events</p>
          <br />
          <div id="nav.left.footer" class="bottomArrow">
            <img src="~/assets/svg/arrow-down.svg" />
          </div>
        </div>
      </div>

      <div id="nav.right" class="relative right">
        <div id="nav.right.header" class="flex rightheader">
          <img
            @click="closeNav"
            id="closeButton"
            class="closeButton"
            src="~/assets/svg/Close Menu icon Red.svg"
          />
        </div>
        <div id="nav.right.content" class="relative wrap rightContentItems">
          <div id="academics">
            <h4>Academics</h4>
            <!-- create dynmaic loading -->
            <ul>
              <li><a href="">Our Faculty</a></li>
              <li><a href="">Our Learning Model</a></li>
              <li><a href="">Programs &amp;amp; Degrees</a></li>
              <li><a href="">Honors Program</a></li>
              <li><a href="">Catalog</a></li>
            </ul>
          </div>
          <div id="church_faith">
            <h4>Church &amp;amp; Faith</h4>
            <ul>
              <li><a href="">Church Alignment</a></li>
              <li><a href="">YSA Stake &amp;amp; Wards</a></li>
              <li><a href="">Institute of Religion</a></li>
              <li><a href="">Missionaries</a></li>
            </ul>
          </div>
          <div id="giving">
            <h4>Giving</h4>
            <ul>
              <li>
                <a href="https://secure.svu.edu/donate/">Make a Donation</a>
              </li>
              <li><a href="">Why Give? *</a></li>
              <li>
                <a href="https://svu.edu/giving/#priorities">Ways to Give</a>
              </li>
              <!--<li><a href="">Capital Projects *</a></li>-->
            </ul>
          </div>
          <div id="admissions">
            <h4>Admissions</h4>
            <ul>
              <li><a href="https://svu.edu/application/">Apply Now</a></li>
              <li>
                <a href="https://svu.edu/admissions/contact/"
                  >Admissions Team</a
                >
              </li>
              <li>
                <a href="https://svu.edu/admissions/#apply">How to Apply</a>
              </li>
              <li>
                <a href="https://svu.edu/admissions/enrollment/"
                  >How to Enroll</a
                >
              </li>
              <li>
                <a href="https://svu.edu/admissions/visit/">Visit Campus</a>
              </li>
            </ul>
          </div>
          <div id="campus_life">
            <h4>Campus Life</h4>
            <ul>
              <li><a href="">Our Campus *</a></li>
              <li>
                <a href="https://svu.edu/campus-life/code-of-honor/"
                  >Code of Conduct</a
                >
              </li>
              <li>
                <a href="https://svu.edu/campus-life/student-success/"
                  >Student Services</a
                >
              </li>
              <li>
                <a href="https://svu.edu/campus-life/dining/">Food Services</a>
              </li>
              <li>
                <a href="https://svu.edu/campus-life/housing/"
                  >University Housing</a
                >
              </li>
              <li>
                <a href="https://svu.edu/about/location/">Explore Virginia</a>
              </li>
            </ul>
          </div>
          <div id="shop">
            <h4>Shop</h4>
            <ul>
              <li><a href="https://gear.svu.edu">Shop Athletics Gear</a></li>
              <li>
                <a href="https://svu.textbookx.com/institutional/index.php"
                  >Online Bookstore</a
                >
              </li>
              <li>
                <a href="https://svu.merchorders.com/">Online Giftshop</a>
              </li>
              <li><a href="https://photos.svu.edu/">Photo Store</a></li>
            </ul>
          </div>
          <div id="tuition_aid">
            <h4>Tuition &amp; Aid</h4>
            <ul>
              <li>
                <a href="https://svu.edu/admissions/financial-services/"
                  >Financial Aid Team</a
                >
              </li>
              <li>
                <a href="https://svu.edu/admissions/scholarships-and-aid/"
                  >Scholarships &amp; Aid</a
                >
              </li>
              <li>
                <a href="https://svu.edu/admissions/tuition-and-payments/"
                  >Tution &amp; Payments</a
                >
              </li>
              <li>
                <a href="https://svu.edu/admissions/scholarships-and-aid/"
                  >About the FAFSA</a
                >
              </li>
              <!-- duplicate -->
            </ul>
          </div>
          <div id="popular_programs">
            <h4>Popular Programs</h4>
            <!-- irregularities in domain names should be addressed in new website -->
            <ul>
              <li><a href="https://art.svu.edu/">Art + Design</a></li>
              <li>
                <a href="https://svu.edu/campus-life/athletics/">Athletics</a>
              </li>
              <!-- mulitiple athletics pages -->
              <li><a href="https://esports.svu.edu/">Esports</a></li>
              <li><a href="https://music.svu.edu/">Music</a></li>
              <li>
                <a href="https://svu.edu/campus-life/marching-band/"
                  >Marching Band</a
                >
              </li>
              <!--<li><a href="">Student Leadership *</a></li>-->
              <li>
                <a href="https://svu.edu/campus-life/theatre/">Theatre</a>
              </li>
              <li>
                <a href="https://svu.edu/academics/programs/pre-law/"
                  >Pre-Law</a
                >
              </li>
              <li>
                <a href="https://catalog.svu.edu/concentrations/pre-medical/"
                  >Pre-Med</a
                >
              </li>
              <!-- irregularity from pre law  -->
            </ul>
          </div>
          <div id="tools">
            <h4>Tools</h4>
            <ul>
              <!--<li><a href="https://svu.edu/about/alumni/">Alumni</a></li>-->
              <li><a href="https://svu.edu/canvas/">Canvas</a></li>
              <li><a href="https://calendar.svu.edu/">Calendars</a></li>
              <li><a href="https://catalog.svu.edu/">Catalog</a></li>
              <li><a href="https://svu.edu/directory/">Directory</a></li>
              <li><a href="https://svu.edu/employment/">Employment</a></li>
              <!--<li><a href="">Knight App *</a></li>-->
              <li>
                <a href="https://my.svu.edu/ics">my<strong>svu</strong></a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div id="left-background" class="bg bg-left"></div>
    <div id="right-background" class="bg bg-right"></div>
  </nav>

</template>

<script>
export default {
  methods: {
    closeNav() {
      const nav = document.getElementById("nav");

      const leftBg = document.getElementById("left-background");
      const rightBg = document.getElementById("right-background");

      nav.style.display = "none";

      leftBg.style.width = 0;
      rightBg.style.width = 0;
    },
    openNav() {
      
    }
  }
}
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

nav {
  max-width: 1600px;
  margin: 0 auto;
  min-height: 100vh;
}

.bg {
  height: 100%;
  position: absolute;
  z-index: -2;
  transition: .3s all ease;
}

.bg-left {
  background-color: #9e1b32;
  top: 0;
  left: 0;
  width: 50%;
  z-index: -1;
}

.bg-right {
  top: 0;
  right: 0;
  width: 100%;
  background-color: white;
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
.topalignChild:not(:last-child) {
  margin-right: 10px;
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
  grid-template-columns: 0.3333fr 0.3333fr 0.3333fr;
  gap: 20px 44px;
  padding: 10% 5% 5% 8%;
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

.socialCircles {
  width: 160px;
  height: 25px;
  display: flex;
  justify-content: space-between;
}
.social-svg {
  height: 25px;
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
