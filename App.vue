<template>
  <div class="container-fluid">
    <!-- <div class="col-sm-1 text-left">
      <div class="well">Basic Well</div>
      <div class="well">Basic Well</div>
      <div class="well">Basic Well</div>
      <div class="well">Basic Well</div>
      <div class="well">Basic Well</div>
    </div> -->

    <div id="left"></div>
    <div id="right"></div>
    <div id="top"></div>
    <div id="bottom"></div>

    <div class="app">
      <!-- Put a box on top of navbar-->
      <nav class="navbar navbar">
        <div class="container-fluid">
          <div class="navbar-header">
            <button
              type="button"
              class="navbar-toggle"
              data-toggle="collapse"
              data-target="#myNavbar"
            >
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
            </button>
          </div>
          <div class="collapse navbar-collapse" id="myNavbar">
            <ul class="nav navbar-nav navbar-left">
              <img src="@/assets/Logo.png" />
            </ul>
            <ul class="nav navbar-nav navbar-right">
              <li><a href="#">home</a></li>

              <li class="active"><a href="#">resources</a></li>
              <li><a href="#">chat</a></li>
              <li>
                <a class="number" href="#"><u>+1-800-273-TALK</u></a>
              </li>
            </ul>
          </div>
        </div>
      </nav>

      <div class="row content">
        <div class="wrapper">
          <div id="Resources">resources</div>
          <img
            class="search-icon"
            src="data:image/svg+xml;utf8;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iaXNvLTg4NTktMSI/Pgo8IS0tIEdlbmVyYXRvcjogQWRvYmUgSWxsdXN0cmF0b3IgMTkuMC4wLCBTVkcgRXhwb3J0IFBsdWctSW4gLiBTVkcgVmVyc2lvbjogNi4wMCBCdWlsZCAwKSAgLS0+CjxzdmcgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIgdmVyc2lvbj0iMS4xIiBpZD0iQ2FwYV8xIiB4PSIwcHgiIHk9IjBweCIgdmlld0JveD0iMCAwIDU2Ljk2NiA1Ni45NjYiIHN0eWxlPSJlbmFibGUtYmFja2dyb3VuZDpuZXcgMCAwIDU2Ljk2NiA1Ni45NjY7IiB4bWw6c3BhY2U9InByZXNlcnZlIiB3aWR0aD0iMTZweCIgaGVpZ2h0PSIxNnB4Ij4KPHBhdGggZD0iTTU1LjE0Niw1MS44ODdMNDEuNTg4LDM3Ljc4NmMzLjQ4Ni00LjE0NCw1LjM5Ni05LjM1OCw1LjM5Ni0xNC43ODZjMC0xMi42ODItMTAuMzE4LTIzLTIzLTIzcy0yMywxMC4zMTgtMjMsMjMgIHMxMC4zMTgsMjMsMjMsMjNjNC43NjEsMCw5LjI5OC0xLjQzNiwxMy4xNzctNC4xNjJsMTMuNjYxLDE0LjIwOGMwLjU3MSwwLjU5MywxLjMzOSwwLjkyLDIuMTYyLDAuOTIgIGMwLjc3OSwwLDEuNTE4LTAuMjk3LDIuMDc5LTAuODM3QzU2LjI1NSw1NC45ODIsNTYuMjkzLDUzLjA4LDU1LjE0Niw1MS44ODd6IE0yMy45ODQsNmM5LjM3NCwwLDE3LDcuNjI2LDE3LDE3cy03LjYyNiwxNy0xNywxNyAgcy0xNy03LjYyNi0xNy0xN1MxNC42MSw2LDIzLjk4NCw2eiIgZmlsbD0iIzAwMDAwMCIvPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8Zz4KPC9nPgo8L3N2Zz4K"
          />
          <input class="search" placeholder="search" type="text" />
        </div>

        <span>
          <div class="well" id="first">
            <h2>
              benefits of exercise on mental health
              <h4>
                <u
                  ><a
                    class="inWell"
                    href="https://www.helpguide.org/articles/healthy-living/the-mental-health-benefits-of-exercise.htm"
                    target="_blank"
                    >read blog</a
                  ></u
                >
              </h4>
            </h2>
          </div>
          <div class="well" id="second">
            <h2>
              moderation - why do we do what we do
              <h4>
                <u
                  ><a
                    class="inWell"
                    href="https://healthyeating.sfgate.com/importance-moderation-1990.html"
                    target="_blank"
                    >read blog</a
                  ></u
                >
              </h4>
            </h2>
          </div>
          <div class="well" id="third">
            <h2>
              31 tips to boost your mental health
              <h4>
                <u
                  ><a
                    class="inWell"
                    href="https://www.mhanational.org/31-tips-boost-your-mental-health"
                    target="_blank"
                    >read blog</a
                  ></u
                >
              </h4>
            </h2>
          </div></span
        >
        <article>
          <header class="tabs">
            <ul>
              <li v-for="(tab, index) in tabs" :key="index">
                <div
                  class="nav-item"
                  :id="{ name: tab.name }"
                  :class="{ 'is-active': tab.isActive }"
                  @click="selectTab(tab)"
                >
                  {{ tab.name }}
                </div>
              </li>
            </ul>
          </header>
          <section class="tabs-details">
            <slot></slot>
          </section>
        </article>

        <Tabs class="tabs">
          <Tab name="activities" id="activities" selected="true">
            <a href="https://www.netflix.com/" target="_blank">
              <img src="@/assets/Netflix.png" id="Netflix"
            /></a>

            <a
              href="https://www.reidhealth.org/blog/mental-health"
              target="_blank"
            >
              <img src="@/assets/StressBall.png" id="StressBall"
            /></a>

            <!--Gotta fix link--><a
              href="http://endeavorga.org/?video-arcade-games-online/"
              target="_blank"
            >
              <img src="@/assets/Arcade.png" id="Arcade"
            /></a>

            <a
              href="https://www.portstluciehospitalinc.com/10-journaling-prompts-for-mental-health/"
              target="_blank"
            >
              <img src="@/assets/Journal.png" id="Journal"
            /></a>

            <a
              href="https://www.bupa.co.uk/health-information/exercise-fitness/types-of-exercise"
              target="_blank"
            >
              <img src="@/assets/Exercise.png" id="Exercise"
            /></a>

            <a
              href="https://www.livekindly.co/7-surprising-ways-cooking-can-boost-your-mental-health/#:~:text=%E2%80%9CCooking%20at%20home%2C%20or%20other,%2C%20themselves%20or%20loved%20ones%2C%E2%80%9D"
              target="_blank"
            >
              <img src="@/assets/Cooking.png" id="Cooking"
            /></a>

            <h5>
              <a href="#" class="More">see more </a>
              <a href="#" class="More"><img src="@/assets/arrow.png" /></a>
            </h5>
          </Tab>

          <Tab name="healthcare" id="healthcare">
            <a href="https://www.teladoc.com/therapy/" target="_blank">
              <img src="@/assets/healthcare.png" id="HealthCare"
            /></a>

            <a href="https://www.teladoc.com/therapy/" target="_blank">
              <img src="@/assets/healthcare.png" id="HealthCare2"
            /></a>

            <a href="https://www.teladoc.com/therapy/" target="_blank">
              <img src="@/assets/healthcare.png" id="HealthCare2"
            /></a>

            <a href="https://www.teladoc.com/therapy/" target="_blank">
              <img src="@/assets/healthcare.png" id="HealthCare"
            /></a>

            <a href="https://www.teladoc.com/therapy/" target="_blank">
              <img src="@/assets/healthcare.png" id="HealthCare2"
            /></a>

            <a href="https://www.teladoc.com/therapy/" target="_blank">
              <img src="@/assets/healthcare.png" id="HealthCare2"
            /></a>

            <h5>
              <a href="#" class="More">see more </a>
              <a href="#" class="More"><img src="@/assets/arrow.png" /></a>
            </h5>
          </Tab>

          <Tab name="research" id="research">
            <a
              href="https://onlinelibrary.wiley.com/journal/17461405"
              target="_blank"
            >
              <img src="@/assets/research.png" id="Research"
            /></a>

            <a
              href="https://onlinelibrary.wiley.com/journal/17461405"
              target="_blank"
            >
              <img src="@/assets/research.png" id="Research2"
            /></a>

            <a
              href="https://onlinelibrary.wiley.com/journal/17461405"
              target="_blank"
            >
              <img src="@/assets/research.png" id="Research2"
            /></a>

            <a
              href="https://onlinelibrary.wiley.com/journal/17461405"
              target="_blank"
            >
              <img src="@/assets/research.png" id="Research"
            /></a>

            <a
              href="https://onlinelibrary.wiley.com/journal/17461405"
              target="_blank"
            >
              <img src="@/assets/research.png" id="Research2"
            /></a>

            <a
              href="https://onlinelibrary.wiley.com/journal/17461405"
              target="_blank"
            >
              <img src="@/assets/research.png" id="Research2"
            /></a>

            <h5>
              <a href="#" class="More">see more </a>
              <a href="#" class="More"><img src="@/assets/arrow.png" /></a>
            </h5>
          </Tab>

          <Tab name="crowdfunding" id="crowdfunding">
            <a
              href="https://www.gofundme.com/c/blog/mental-health-fundraising"
              target="_blank"
            >
              <img src="@/assets/crowdfunding.png" id="Crowdfunding"
            /></a>

            <a
              href="https://www.gofundme.com/c/blog/mental-health-fundraising"
              target="_blank"
            >
              <img src="@/assets/crowdfunding.png" id="Crowdfunding2"
            /></a>

            <a
              href="https://www.gofundme.com/c/blog/mental-health-fundraising"
              target="_blank"
            >
              <img src="@/assets/crowdfunding.png" id="Crowdfunding2"
            /></a>

            <a
              href="https://www.gofundme.com/c/blog/mental-health-fundraising"
              target="_blank"
            >
              <img src="@/assets/crowdfunding.png" id="Crowdfunding"
            /></a>

            <a
              href="https://www.gofundme.com/c/blog/mental-health-fundraising"
              target="_blank"
            >
              <img src="@/assets/crowdfunding.png" id="Crowdfunding2"
            /></a>

            <a
              href="https://www.gofundme.com/c/blog/mental-health-fundraising"
              target="_blank"
            >
              <img src="@/assets/crowdfunding.png" id="Crowdfunding2"
            /></a>

            <h5>
              <a href="#" class="More">see more </a>
              <a href="#" class="More"><img src="@/assets/arrow.png" /></a>
            </h5>
          </Tab>

          <Tab name="hotlines" id="hotlines">
            <a
              href="https://www.asafeplaceonline.com/?gclid=Cj0KCQjwub-HBhCyARIsAPctr7xRVAiSs8fVR_n8QFSbcni68MT2uQBpyHsd0B-ROHZ2qyyROuNUgrsaAh_QEALw_wcB"
              target="_blank"
            >
              <img src="@/assets/hotlines.png" id="Hotlines"
            /></a>

            <a
              href="https://www.asafeplaceonline.com/?gclid=Cj0KCQjwub-HBhCyARIsAPctr7xRVAiSs8fVR_n8QFSbcni68MT2uQBpyHsd0B-ROHZ2qyyROuNUgrsaAh_QEALw_wcB"
              target="_blank"
            >
              <img src="@/assets/hotlines.png" id="Hotlines2"
            /></a>

            <a
              href="https://www.asafeplaceonline.com/?gclid=Cj0KCQjwub-HBhCyARIsAPctr7xRVAiSs8fVR_n8QFSbcni68MT2uQBpyHsd0B-ROHZ2qyyROuNUgrsaAh_QEALw_wcB"
              target="_blank"
            >
              <img src="@/assets/hotlines.png" id="Hotlines2"
            /></a>

            <a
              href="https://www.asafeplaceonline.com/?gclid=Cj0KCQjwub-HBhCyARIsAPctr7xRVAiSs8fVR_n8QFSbcni68MT2uQBpyHsd0B-ROHZ2qyyROuNUgrsaAh_QEALw_wcB"
              target="_blank"
            >
              <img src="@/assets/hotlines.png" id="Hotlines"
            /></a>

            <a
              href="https://www.asafeplaceonline.com/?gclid=Cj0KCQjwub-HBhCyARIsAPctr7xRVAiSs8fVR_n8QFSbcni68MT2uQBpyHsd0B-ROHZ2qyyROuNUgrsaAh_QEALw_wcB"
              target="_blank"
            >
              <img src="@/assets/hotlines.png" id="Hotlines2"
            /></a>

            <a
              href="https://www.asafeplaceonline.com/?gclid=Cj0KCQjwub-HBhCyARIsAPctr7xRVAiSs8fVR_n8QFSbcni68MT2uQBpyHsd0B-ROHZ2qyyROuNUgrsaAh_QEALw_wcB"
              target="_blank"
            >
              <img src="@/assets/hotlines.png" id="Hotlines2"
            /></a>

            <h5>
              <a href="#" class="More">see more </a>
              <a href="#" class="More"><img src="@/assets/arrow.png" /></a>
            </h5>
          </Tab>

          <Tab name="facts" id="facts">
            <a
              href="https://www.mentalhealth.gov/basics/mental-health-myths-facts"
              target="_blank"
            >
              <img src="@/assets/facts.png" id="Facts"
            /></a>

            <a
              href="https://www.mentalhealth.gov/basics/mental-health-myths-facts"
              target="_blank"
            >
              <img src="@/assets/facts.png" id="Facts2"
            /></a>

            <a
              href="https://www.mentalhealth.gov/basics/mental-health-myths-facts"
              target="_blank"
            >
              <img src="@/assets/facts.png" id="Facts2"
            /></a>

            <a
              href="https://www.mentalhealth.gov/basics/mental-health-myths-facts"
              target="_blank"
            >
              <img src="@/assets/facts.png" id="Facts"
            /></a>

            <a
              href="https://www.mentalhealth.gov/basics/mental-health-myths-facts"
              target="_blank"
            >
              <img src="@/assets/facts.png" id="Facts2"
            /></a>

            <a
              href="https://www.mentalhealth.gov/basics/mental-health-myths-facts"
              target="_blank"
            >
              <img src="@/assets/facts.png" id="Facts2"
            /></a>

            <h5>
              <a href="#" class="More">see more </a>
              <a href="#" class="More"><img src="@/assets/arrow.png" /></a>
            </h5>
          </Tab>
        </Tabs>
      </div>
    </div>

    <div class="testimonials">
      <img src="@/assets/Review-Seth.png" id="Seth" />
      <img src="@/assets/Review-Mary.png" id="Mary" />
      <img src="@/assets/Review-Jennifer.png" id="Jennifer" />
      <img src="@/assets/Review-Chat.png" id="Chat" />
      <img src="@/assets/Review-Chat2.png" id="Chat2" />
    </div>

    <!-- <div class="col-sm-1 text-left">
      <div class="well">Basic Well</div>
      <div class="well">Basic Well</div>
      <div class="well">Basic Well</div>
      <div class="well">Basic Well</div>
      <div class="well">Basic Well</div>
    </div> -->
  </div>
</template>

<style lang="scss">
@import "@/global-styles/colors.scss";
@import "@/global-styles/typography.scss";

body {
  background-color: $white;
}

h1 {
  @include heading-1($black);
  padding-bottom: 3rem;
  font-family: $font-family;
}

h2 {
  @include heading-2($white);
}

h3 {
  @include heading-3($black);
  padding-top: 0;
  padding-bottom: 2rem;
}

h4 {
  @include heading-4($white);
  border: 2px solid $white;
  border-radius: 6px;
  width: 60%;
  margin-left: 5rem;
}

h5 {
  @include heading-2-right($white);
  margin-top: 30px;
}

p {
  @include heading-2-right($white);
}

a {
  color: $black;

  &.More {
    color: $white;
    &:hover {
      text-decoration: none;
    }
  }

  &.number {
    color: $purple;
  }
  &.inWell {
    color: $white;
    &:hover {
      color: $black;
    }
  }
}

li {
  @include medium-text($black);

  margin-right: 70px;

  &.active {
    border-bottom: 3px solid $light-purple;
  }
}

#Seth,
#Mary,
#Jennifer {
  margin-top: 30rem;
  margin-bottom: 100px;
  border: 1px solid grey;
  border-radius: 5px;
}

#Seth {
  margin-left: 12rem;
}

#Mary {
  margin-left: 15rem;
}

#Jennifer {
  margin-left: 15rem;
}

#Chat {
  margin-left: 30rem;
  margin-bottom: 100px;
  width: 17%;
}

#Chat2 {
  margin-left: 35rem;
  margin-bottom: 100px;
  width: 17%;
}

#top,
#bottom,
#left,
#right {
  background: #c7b9ff; //Prob diff color
  margin: 0;
  padding: 0;
}
#left,
#right {
  top: 0;
  bottom: 0;
  width: 30px;
  position: fixed;
}
#left {
  left: 0;
}
#right {
  right: 0;
}

#top,
#bottom {
  left: 0;
  right: 0;
  height: 30px;
}
#top {
  top: 0;
}
#bottom {
  bottom: 0;
  position: fixed;
}

#Resources {
  font-size: 50px;
  color: $black;
  font-family: $font-family;
  font-weight: bold;
  //text-shadow: 0px 4px 3px rgba(0, 0, 0, 0.4);
  margin-left: 60px;
}

#Netflix,
#StressBall,
#Arcade,
#Journal,
#Exercise,
#Cooking,
#HealthCare,
#HealthCare2,
#Research,
#Research2,
#Crowdfunding,
#Crowdfunding2,
#Hotlines,
#Hotlines2,
#Facts,
#Facts2 {
  width: 30%;
  margin-bottom: 80px;
  margin-top: 20px;
  border-radius: 5px;
}
#StressBall,
#Arcade,
#Exercise,
#Cooking,
#HealthCare2,
#Research2,
#Crowdfunding2,
#Hotlines2,
#Facts2 {
  margin-left: 65px;
}

.app {
  font-family: $font-family;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: $black;
  // border-left: 3px solid black;
  // border-right: 3px solid black;
  //border-top: 3px solid black;
  //border-bottom: 3px solid black;
  //box-shadow: 0px 0px 5px black;
  display: relative;
  margin-right: 15px;
  margin-left: 15px;
  margin-top: 0px;
  margin-bottom: 0px;
  background-image: linear-gradient(
    0deg,
    rgba(255, 0, 0, 0) 85%,
    92%,
    rgb(218, 194, 245)
  );
}

/* Remove the navbar's default margin-bottom and rounded borders */
.navbar {
  margin-bottom: 0px;
  padding-bottom: 0rem;
  margin-top: 0px;
  padding-top: 8px;
  box-shadow: 0px 0px 1px rgb(209, 209, 209);
  height: 70px;

  //border-top: 15px solid #a68bd1;
  border-radius: 0px;
  background-color: $white;
  font-family: $font-family;
}

.navbar-inverse .navbar-brand,
.navbar-inverse .navbar-text {
  color: $white;
}

.navbar-inverse .navbar-nav > li > a {
  color: $white;
}

/* Set height of the grid so .sidenav can be 100% (adjust as needed) */
.row.content {
  height: 667px;
}

/* Set white background color and 100% height */
.sidenav {
  padding-top: 20px;
  background-color: $white;
  height: 100%;
}

.tabs {
  padding-top: 4rem;
  margin-left: 60px;
  margin-right: 60px;
  padding-bottom: 0;
  margin-bottom: 0;
}

.tabs-details {
  margin: 0;
  padding: 0;
  // padding: 1px;
  // background-color: $purple;
  // margin-left: 60px;
  // margin-right: 60px;
  // margin-bottom: 0;
  // border-radius: 5px;
  // box-shadow: 10px 10px 5px rgb(175, 174, 174), 0px 0px 10px 3px $light-purple;
}

#activities,
#healthcare,
#research,
#crowdfunding,
#hotlines,
#facts {
  background-color: $purple;
  margin-top: -20px;
  padding: 20px;
  margin-left: 60px;
  margin-right: 60px;
  border-top-left-radius: 0;
  border-top-right-radius: 5px;
  border-bottom-left-radius: 5px;
  border-bottom-right-radius: 5px;
  box-shadow: 10px 10px 5px rgb(175, 174, 174), 0px 0px 10px 3px $light-purple;
}

ul {
  display: flex;
  padding: 0;
  list-style: none;
  margin: 0;

  li {
    margin-left: 0px;
    margin-right: 0px;
    margin-bottom: 0;
    padding: 0;
  }

  .nav-item {
    cursor: pointer;
    color: $black;
    margin: 0;
    padding-top: 10px;
    padding-left: 20px;
    padding-right: 20px;
    padding-bottom: 10px;
    border-radius: 6px;
    border: 1.5px solid $purple;
    //border: 2px solid black;
    &:hover {
      color: $purple;
    }
    &.healthcare {
      border: 2px solid $purple;
    }

    &.is-active {
      //Need to make bottom touch line
      color: $white;
      background-color: $purple;
      border-top-left-radius: 6px;
      border-top-right-radius: 6px;
      border-bottom-left-radius: 0;
      border-bottom-right-radius: 0;
      //   padding-left: 15px;
      //   padding-right: 15px;
    }
  }
}

#first {
  margin-left: 60px;
}
#second,
#third {
  margin-left: 140px;
}

.well {
  //visibility: hidden;
  border-color: blue;
  border-radius: 5px;
  box-shadow: 4px 5px 5px rgb(175, 174, 174);
  background-color: $purple;
  margin-top: 20px;
  display: inline-flex;
  width: 19.1%;
  height: 18%;

  margin-bottom: 0;
}
.wrapper {
  position: relative;
  display: flex;
  min-width: 100px;
  padding-top: 0px;
}

.search {
  border: 0px solid;
  border-radius: 10px;
  height: 30px;
  width: 28.5%;
  padding: 2px 23px 2px 30px;
  margin-left: 65rem;
  margin-top: 2.85rem;
  outline: 0;
  background-color: #e0e0e0f3;
}

::placeholder {
  /* Chrome, Firefox, Opera, Safari 10.1+ */
  color: grey;
  font-size: 17px;
  padding-left: 3px;
}

.search:hover,
.search:focus {
  border: 0px solid black;
  background-color: rgb(240, 240, 245);
  transition-duration: 420ms;
}

.search-icon {
  position: absolute;
  top: 3.6rem;
  left: 96rem;
  width: 16px;
}

.clear-icon {
  position: absolute;
  top: 35px;
  right: 12.5rem;
  width: 17px;
  cursor: pointer;
  //visibility: hidden;
}

@media screen and (max-width: 767px) {
  .sidenav {
    height: auto;
    padding: 15px;
  }
  .row.content {
    height: auto;
  }
}
</style>

<script>
import Tab from "@/components/Tab";
//import Tabs from "@/components/Tabs";
export default {
  name: "App",
  data: () => {
    return {
      tabs: [],
    };
  },
  components: {
    Tab,
    //Tabs,
  },
  methods: {
    selectTab(selectedTab) {
      this.tabs.forEach((tab) => {
        tab.isActive = tab.name === selectedTab.name;
      });
    },
  },
  created() {
    this.tabs = this.$children;
  },
};
</script>