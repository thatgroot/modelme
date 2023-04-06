<script lang="ts">
  import { createEventDispatcher } from "svelte";
  import Checkbox from "../checkbox.svelte";
  import more_svg from "../../../assets/icons/more.svg";

  // props export for below
  export let images: Array<string> = [];
  export let title: string;
  // author of the image
  export let author: string;
  // text for the image
  export let alt: string;

  export let tags: Array<string> = [];

  const dispatch = createEventDispatcher();

  // create a type that only accepts links with image extenstion like .png .jpeg, etc
</script>

<div class="inline-flex flex-col items-start justify-start space-y-4">
  <div class="flex relative h-72 w-80">
    <div
      class="absolute left-0 right-0 inline-flex items-center justify-between p-2"
    >
      <Checkbox size="small" border="border-[#ffffff]" />

      <img src={more_svg} alt="more" class="w-4 h-4 cursor-pointer" />
    </div>

    {#if images.length > 1}
      <!-- svelte-ignore a11y-click-events-have-key-events -->
      <div
        class="h-full w-1/2 bg-center bg-cover"
        on:click={() => {
          dispatch("imageclick", { value: true });
        }}
        style="background-image:url({images.length > 0
          ? images[0]
          : 'https://via.placeholder.com/149x149'})"
      />

      <div class="flex flex-col w-1/2">
        <!-- svelte-ignore a11y-click-events-have-key-events -->
        <div
          on:click={() => {
            dispatch("imageclick", { value: true });
          }}
          class="h-full w-full bg-center bg-cover"
          style="background-image:url({images.length > 0
            ? images[1]
            : 'https://via.placeholder.com/149x149'})"
        />

        <!-- svelte-ignore a11y-click-events-have-key-events -->
        <div
          on:click={() => {
            dispatch("imageclick", { value: true });
          }}
          class="h-full w-full bg-center bg-cover"
          style="background-image:url({images.length > 0
            ? images[2]
            : 'https://via.placeholder.com/149x149'})"
        />
      </div>
    {:else}
      <!-- svelte-ignore a11y-click-events-have-key-events -->
      <div
        class="h-full w-full bg-center bg-cover"
        on:click={() => {
          dispatch("imageclick", { value: true });
        }}
        style="background-image:url({images.length > 0
          ? images[0]
          : 'https://via.placeholder.com/149x149'})"
      />
    {/if}
  </div>
  <div class="flex flex-col items-start justify-start gap-3">
    <div class="flex flex-col items-start justify-start gap-2">
      <span class="text-2xl font-medium leading-[1.2] text-[#232323]">
        This is Folder
      </span>
      <span class="text-lg text-[#9A9A9A] leading-[1.2]">
        1 image ⏤ Created by You
      </span>
    </div>
    <div class="flex items-start justify-start gap-2 py-1">
      <span class="bg-gray-100 px-3 text-lg leading-relaxed text-[#6C6C6C]"
        >Tag</span
      >
      <span class="bg-gray-100 px-3 text-lg leading-relaxed text-[#6C6C6C]"
        >Tag</span
      >
      <span class="bg-gray-100 px-3 text-lg leading-relaxed text-[#6C6C6C]"
        >Tag</span
      >
    </div>
  </div>
</div>
