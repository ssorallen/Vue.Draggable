<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <div class="container ">
      <ul class="nav nav-tabs" role="tablist">
        <li class="nav-item">
          <a
            class="nav-link active"
            data-toggle="tab"
            href="#simple"
            role="tab"
            aria-controls="profile"
            aria-selected="true"
            >Simple</a
          >
        </li>

        <li class="nav-item">
          <a
            class="nav-link"
            data-toggle="tab"
            href="#twoLists"
            role="tab"
            aria-controls="profile"
            aria-selected="false"
            >Two Lists</a
          >
        </li>

        <li class="nav-item">
          <a
            class="nav-link"
            data-toggle="tab"
            href="#clone"
            role="tab"
            aria-controls="profile"
            aria-selected="false"
            >Clone</a
          >
        </li>

        <li class="nav-item">
          <a
            class="nav-link"
            data-toggle="tab"
            href="#handler"
            role="tab"
            aria-controls="profile"
            aria-selected="false"
            >Handler</a
          >
        </li>

        <li class="nav-item">
          <a
            class="nav-link"
            data-toggle="tab"
            href="#transition"
            role="tab"
            aria-controls="profile"
            aria-selected="false"
            >Transition</a
          >
        </li>

        <li class="nav-item">
          <a
            class="nav-link"
            data-toggle="tab"
            href="#transitions"
            role="tab"
            aria-controls="profile"
            aria-selected="false"
            >Transitions</a
          >
        </li>

        <li class="nav-item">
          <a
            class="nav-link"
            data-toggle="tab"
            href="#footerslot"
            role="tab"
            aria-controls="profile"
            aria-selected="false"
            >Footer slot</a
          >
        </li>

        <li class="nav-item">
          <a
            class="nav-link"
            data-toggle="tab"
            href="#headerslot"
            role="tab"
            aria-controls="profile"
            aria-selected="false"
            >Header slot</a
          >
        </li>
      </ul>

      <div class="tab-content" id="tab-content">
        <div
          class="tab-pane show active"
          id="simple"
          role="tabpanel"
          aria-labelledby="profile-tab"
        >
          <simple />
        </div>

        <div
          class="tab-pane show"
          id="twoLists"
          role="tabpanel"
          aria-labelledby="profile-tab"
        >
          <twoLists />
        </div>

        <div
          class="tab-pane show"
          id="clone"
          role="tabpanel"
          aria-labelledby="profile-tab"
        >
          <clone />
        </div>

        <div
          class="tab-pane show"
          id="footerslot"
          role="tabpanel"
          aria-labelledby="profile-tab"
        >
          <footerslot />
        </div>

        <div
          class="tab-pane show"
          id="headerslot"
          role="tabpanel"
          aria-labelledby="profile-tab"
        >
          <headerslot />
        </div>

        <div
          class="tab-pane show"
          id="handler"
          role="tabpanel"
          aria-labelledby="profile-tab"
        >
          <handler />
        </div>

        <div
          class="tab-pane show"
          id="transition"
          role="tabpanel"
          aria-labelledby="profile-tab"
        >
          <transition-example />
        </div>

        <div
          class="tab-pane show"
          id="transitions"
          role="tabpanel"
          aria-labelledby="profile-tab"
        >
          <transition-example-2 />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import simple from "./components/simple";
import twoLists from "./components/two-lists";
import clone from "./components/clone";
import footerslot from "./components/footerslot";
import headerslot from "./components/headerslot";
import handler from "./components/handler";
import transitionExample from "./components/transition-example";
import transitionExample2 from "./components/transition-example-2";

export default {
  name: "app",
  components: {
    simple,
    twoLists,
    clone,
    footerslot,
    headerslot,
    handler,
    transitionExample,
    transitionExample2
  }
};
</script>

<style>
.main-application {
  width: 400px;
}

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
