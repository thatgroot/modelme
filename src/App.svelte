<script lang="ts">
  import MainNavigation from "./lib/components/navigation/main-navigation.svelte";
  import GeneratePage from "./routes/generate-page.svelte";
  import HistoryPage from "./routes/history-page.svelte";
  import HomePage from "./routes/home-page.svelte";
  import ProfilePage from "./routes/profile-page.svelte";
  import Router from "svelte-spa-router";
  import { push } from "svelte-spa-router";
  import HomeNavigation from "./lib/components/navigation/home-navigation.svelte";

  const routes = {
    "/": HomePage,
    "/history": HistoryPage,
    "/generate": GeneratePage,
    "/profile": ProfilePage,
  };
</script>

<div class="flex flex-col bg-white w-full max-w-[1440px] mx-auto">
  <!-- <MainNavigation /> -->
  <HomeNavigation/>
  <Router {routes} />
</div>
