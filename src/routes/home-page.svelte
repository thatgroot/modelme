<script>
  import HomeGallery from "../lib/components/home/home-gallery.svelte";
  import HomeHowto from "../lib/components/home/home-howto.svelte";
  import HomeIntro from "../lib/components/home/home-intro.svelte";
  import HomePricing from "../lib/components/home/home-pricing.svelte";
  import HomeTeam from "../lib/components/home/home-team.svelte";
  import HomeBanner from "../lib/components/home/home-contact.svelte";
  import Footer from "../lib/components/footer.svelte";
</script>

<div class="flex flex-col justify-start items-end relative">
  <HomeIntro />
  <HomeHowto />
  <HomeGallery />
  <HomePricing />
  <HomeTeam />
  <HomeBanner />
  <Footer/>
</div>
