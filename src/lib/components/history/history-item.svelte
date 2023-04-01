<script lang="ts">
  import { createEventDispatcher } from "svelte";

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
      <div
        class="h-3 w-3 rounded-[3px] border-2 border-white bg-transparent bg-opacity-50"
      />

      <div class="flex gap-1">
        <div class="h-2 w-2 rounded-lg border-2" />
        <div class="h-2 w-2 rounded-lg border-2" />
        <div class="h-2 w-2 rounded-lg border-2" />
      </div>
    </div>
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
      <div
        class="h-full w-full bg-center bg-cover"
        style="background-image:url({images.length > 0
          ? images[1]
          : 'https://via.placeholder.com/149x149'})"
      />

      <div
        class="h-full w-full bg-center bg-cover"
        style="background-image:url({images.length > 0
          ? images[2]
          : 'https://via.placeholder.com/149x149'})"
      />
    </div>
  </div>
  <div class="flex flex-col items-start justify-start space-y-3">
    <div class="Text flex flex-col items-start justify-start space-y-2">
      <p class="Thisis Folder text-2xl font-medium leading-loose text-gray-800">
        This is Folder
      </p>
      <p class="1image ⏤ Created by You text-lg leading-relaxed text-gray-400">
        1 image ⏤ Created by You
      </p>
    </div>
    <div class="flex items-start justify-start gap-2 py-1">
      <p class="bg-gray-100 px-3 text-lg leading-relaxed text-gray-500">Tag</p>
      <p class="bg-gray-100 px-3 text-lg leading-relaxed text-gray-500">Tag</p>
      <p class="bg-gray-100 px-3 text-lg leading-relaxed text-gray-500">Tag</p>
    </div>
  </div>
</div>
