<script lang="ts">
  import GenerateFilters from "../lib/components/generate/generate-filters.svelte";
  import GenerateNavigation from "../lib/components/generate/generate-navigation.svelte";
  import GenerateSidebar from "../lib/components/generate/generate-sidebar.svelte";
  import image_15 from "../assets/15.png";
  import image_16 from "../assets/16.png";
  import image_17 from "../assets/17.png";
  import image_18 from "../assets/18.png";
  import gradient_image from "../assets/gradient.png";
  import Checkbox from "../lib/components/checkbox.svelte";
  import MainNavigation from "../lib/components/navigation/main-navigation.svelte";
  import PageWrapper from "../lib/components/page-wrapper.svelte";
  import Login from "../lib/components/login.svelte";
  let selected_models: Array<any> = [];
</script>

<PageWrapper>
  <MainNavigation />
  <div id="generate-section" class="flex flex-col gap-6">
    <div class="flex flex-col gap-6 mt-4">
      <GenerateNavigation />
    </div>
    <div
      class="flex items-start justify-between gap-6 -ml-[23px] -mr-[23px] w-full"
    >
      <GenerateSidebar />
      <div class="flex flex-col gap-4 items-start justify-start">
        <GenerateFilters />
        <div
          class="flex justify-between items-start w-full flex-grow-0 flex-shrink-0 gap-4 min-h-screen"
        >
          {#each [image_15, image_16, image_17, image_18] as image}
            <div
              class="flex flex-col w-[248.5px] justify-start items-start flex-grow-0 flex-shrink-0 relative gap-2.5"
            >
              <img
                alt="..."
                src={image}
                class="flex-grow-0 flex-shrink-0 w-full h-[350px] object-cover"
              />
              <div
                class="flex-grow-0 flex-shrink-0 w-6 h-6 absolute left-4 top-4"
              >
                <Checkbox
                  name="name"
                  on:change={(e) => {
                    selected_models.push({
                      name: `name_${Math.random()}`,
                      value: e.detail,
                    });
                  }}
                  label=""
                  border="border-[#ffffff]"
                />
              </div>
            </div>
          {/each}
        </div>
        <div
          class="flex justify-start items-center h-24 w-fit fixed bottom-6 gap-4 p-8 bg-[#d8d8d8]"
        >
          <span
            class="z-[999] w-[361px] text-2xl font-medium text-left text-white"
          >
            Go to the History tab to find your generated images
          </span>
          <img
            src={gradient_image}
            alt="..."
            class="absolute left-0 right-0 bottom-0 top-0 flex-grow-0 flex-shrink-0 w-[473px] h-[100px] object-cover"
          />

          <svg
            width="32"
            height="33"
            viewBox="0 0 32 33"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            class="flex-grow-0 flex-shrink-0 w-8 h-8 relative"
            preserveAspectRatio="xMidYMid meet"
          >
            <path
              d="M15.9993 3.1665C8.65268 3.1665 2.66602 9.15317 2.66602 16.4998C2.66602 23.8465 8.65268 29.8332 15.9993 29.8332C23.346 29.8332 29.3327 23.8465 29.3327 16.4998C29.3327 9.15317 23.346 3.1665 15.9993 3.1665ZM20.4793 19.5665C20.866 19.9532 20.866 20.5932 20.4793 20.9798C20.2793 21.1798 20.026 21.2732 19.7727 21.2732C19.5193 21.2732 19.266 21.1798 19.066 20.9798L15.9993 17.9132L12.9327 20.9798C12.7327 21.1798 12.4793 21.2732 12.226 21.2732C11.9727 21.2732 11.7193 21.1798 11.5193 20.9798C11.1327 20.5932 11.1327 19.9532 11.5193 19.5665L14.586 16.4998L11.5193 13.4332C11.1327 13.0465 11.1327 12.4065 11.5193 12.0198C11.906 11.6332 12.546 11.6332 12.9327 12.0198L15.9993 15.0865L19.066 12.0198C19.4527 11.6332 20.0927 11.6332 20.4793 12.0198C20.866 12.4065 20.866 13.0465 20.4793 13.4332L17.4127 16.4998L20.4793 19.5665Z"
              fill="#D2D2E2"
            />
          </svg>
        </div>
      </div>
    </div>
  </div>
</PageWrapper>

<style>
  * {
    font-family: var(--theme-font-family-base, var(--theme-font-family));
  }
</style>
