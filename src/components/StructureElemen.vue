<template>
<div class="container">
    <h3 style="font-size:18.72px; text-align: center; color:#6610f2; font-family: Cinzel, serif; margin-bottom: 20px; margin-top: 20px;">Organization Structure</h3>
  <hr class="bg-primary mb-4 mt-0 d-inline-block mx-auto" style="width: 100px; height:3px;">
  <h1 class="level-1 rectangle">CEO</h1>
  <ol class="level-2-wrapper">
    <li>
      <h2 class="level-2 rectangle">Project Director</h2>
      <ol class="level-3-wrapper">
        <li>
          <h3 class="level-3 rectangle">Developer</h3>
          <ol class="level-4-wrapper">
            <li>
              <h4 class="level-4 rectangle">Android Dev</h4>
            </li>
            <li>
              <h4 class="level-4 rectangle">Back End Dev</h4>
            </li>
            <li>
              <h4 class="level-4 rectangle">Front End Dev</h4>
            </li>
          </ol>
        </li>
        <li>
          <h3 class="level-3 rectangle">Consultant</h3>
          <ol class="level-4-wrapper">
            <li>
              <h4 class="level-4 rectangle">Customer Service</h4>
            </li>
          </ol>
        </li>
      </ol>
    </li>
    <li>
      <h2 class="level-2 rectangle">Education Director</h2>
      <ol class="level-3-wrapper">
        <li>
          <h3 class="level-3 rectangle">Junior Class</h3>
          <ol class="level-4-wrapper">
            <li>
              <h4 class="level-4 rectangle">Web Programmer</h4>
            </li>
            <li>
              <h4 class="level-4 rectangle">Android Dev</h4>
            </li>
            <li>
              <h4 class="level-4 rectangle">Data Science</h4>
            </li>
          </ol>
        </li>
        <li>
          <h3 class="level-3 rectangle">Senior Class</h3>
          <ol class="level-4-wrapper">
            <li>
              <h4 class="level-4 rectangle">Web Programmer</h4>
            </li>
            <li>
              <h4 class="level-4 rectangle">Android Dev</h4>
            </li>
            <li>
              <h4 class="level-4 rectangle">Data Science</h4>
            </li>
          </ol>
        </li>
      </ol>
    </li>
  </ol>
</div>
</template>
<style scoped>
/* RESET STYLES & HELPER CLASSES
–––––––––––––––––––––––––––––––––––––––––––––––––– */

* {
  padding: 0;
  margin-bottom: 20px;
  box-sizing: border-box;
  color: white;
  font-size: 12px;
}

ol {
  list-style: none;
}

body {
  margin: 50px 0 100px;
  margin-bottom: 20px;
  text-align: center;
  font-family: "Inter", sans-serif;
}

.container {
  max-width: 1000px;
  padding: 0 10px;
  margin: 0 auto;
}

.rectangle {
  position: relative;
  padding: 10px;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.15);
}


/* LEVEL-1 STYLES
–––––––––––––––––––––––––––––––––––––––––––––––––– */
.level-1 {
  width: 50%;
  margin: 0 auto 40px;
  background: #6610f2;
}

.level-1::before {
  content: "";
  position: absolute;
  top: 100%;
  left: 50%;
  transform: translateX(-50%);
  width: 2px;
  height: 20px;
  background: black;
}


/* LEVEL-2 STYLES
–––––––––––––––––––––––––––––––––––––––––––––––––– */
.level-2-wrapper {
  position: relative;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
}

.level-2-wrapper::before {
  content: "";
  position: absolute;
  top: -20px;
  left: 25%;
  width: 50%;
  height: 2px;
  background: black;
}

.level-2-wrapper::after {
  display: none;
  content: "";
  position: absolute;
  left: -20px;
  bottom: -20px;
  width: calc(100% + 20px);
  height: 2px;
  background: black;
}

.level-2-wrapper li {
  position: relative;
}

.level-2-wrapper > li::before {
  content: "";
  position: absolute;
  bottom: 100%;
  left: 50%;
  transform: translateX(-50%);
  width: 2px;
  height: 20px;
  background: black;
}

.level-2 {
  width: 70%;
  margin: 0 auto 40px;
  background: #6f1ff1;
}

.level-2::before {
  content: "";
  position: absolute;
  top: 100%;
  left: 50%;
  transform: translateX(-50%);
  width: 2px;
  height: 20px;
  background: black;
}

.level-2::after {
  display: none;
  content: "";
  position: absolute;
  top: 50%;
  left: 0%;
  transform: translate(-100%, -50%);
  width: 20px;
  height: 2px;
  background: black;
}


/* LEVEL-3 STYLES
–––––––––––––––––––––––––––––––––––––––––––––––––– */
.level-3-wrapper {
  position: relative;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-column-gap: 20px;
  width: 90%;
  margin: 0 auto;
}

.level-3-wrapper::before {
  content: "";
  position: absolute;
  top: -20px;
  left: calc(25% - 5px);
  width: calc(50% + 10px);
  height: 2px;
  background: black;
}

.level-3-wrapper > li::before {
  content: "";
  position: absolute;
  top: 0;
  left: 50%;
  transform: translate(-50%, -100%);
  width: 2px;
  height: 20px;
  background: black;
}

.level-3 {
  margin-bottom: 20px;
  background: #6e1fee;
}


/* LEVEL-4 STYLES
–––––––––––––––––––––––––––––––––––––––––––––––––– */
.level-4-wrapper {
  position: relative;
  width: 80%;
  margin-left: auto;
}

.level-4-wrapper::before {
  content: "";
  position: absolute;
  top: -20px;
  left: -20px;
  width: 2px;
  height: calc(100% + 20px);
  background: black;
}

.level-4-wrapper li + li {
  margin-top: 20px;
}

.level-4 {
  font-weight: normal;
  background: #833ff0;
}

.level-4::before {
  content: "";
  position: absolute;
  top: 50%;
  left: 0%;
  transform: translate(-100%, -50%);
  width: 20px;
  height: 2px;
  background: black;
}


/* MQ STYLES
–––––––––––––––––––––––––––––––––––––––––––––––––– */
@media screen and (max-width: 700px) {
  .rectangle {
    padding: 20px 10px;
  }

  .level-1,
  .level-2 {
    width: 100%;
  }

  .level-1 {
    margin-bottom: 20px;
  }

  .level-1::before,
  .level-2-wrapper > li::before {
    display: none;
  }
  
  .level-2-wrapper,
  .level-2-wrapper::after,
  .level-2::after {
    display: block;
  }

  .level-2-wrapper {
    width: 90%;
    margin-left: 10%;
  }

  .level-2-wrapper::before {
    left: -20px;
    width: 2px;
    height: calc(100% + 40px);
  }

  .level-2-wrapper > li:not(:first-child) {
    margin-top: 50px;
  }
}

</style>