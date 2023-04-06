<script lang="ts">
  import GeneratePage from "./routes/generate-page.svelte";
  import HistoryPage from "./routes/history-page.svelte";
  import HomePage from "./routes/home-page.svelte";
  import ProfilePage from "./routes/profile-page.svelte";
  import Router from "svelte-spa-router";

  const routes = {
    "/": HomePage,
    "/history": HistoryPage,
    "/generate": GeneratePage,
    "/profile": ProfilePage,
  };
</script>

<svelte:head>
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin={true} />
  <link
    rel="preload"
    as="style"
    href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Inter:wght@100;200;400;500;600;700;800;900&display=swap"
  />
  <link
    rel="preload"
    href="https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap"
    as="style"
  />

  <link
    rel="stylesheet"
    href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Inter:wght@100;200;400;500;600;700;800;900&display=swap"
  />
  <link
    rel="stylesheet"
    href="https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap"
  />
</svelte:head>
<!-- <MainNavigation /> -->
<Router {routes} />
