<script lang="ts">
  import { onMount } from "svelte";

  export let title: string;
  export let subtitle: string;
  export let instruction: string;
  export let perks: string[];
  export let size: "wide" | "tall" = "tall";
  let gap = "gap-14";
  onMount(() => {
    if (size === "wide") {
      gap = "gap-[55px]";
    } else {
      gap = "gap-[87px]";
    }
  });
</script>

<div
  class="hidden group-hover:flex overflow-hidden right-0 bottom-0 hover:h-full flex-col {gap} items-start z-99 px-[34px] py-10 h-full w-full absolute left-[-1px] top-[-1px] bg-gradient-to-b from-[#4434c9]/80 to-[#4434c9]/40 transition-[height]"
>
  <div class="flex flex-col justify-start items-start relative">
    <span class="text-lg font-semibold text-left text-white">
      {subtitle}
    </span>
    <span class="text-[32px] font-semibold text-left text-white">
      {title}
    </span>
  </div>
  <div class="flex flex-col justify-start items-start relative gap-6">
    {#if instruction}
      <div class="w-[312px] text-lg text-left text-white">
        {instruction}
      </div>
    {/if}

    {#if perks.length > 0}
      <ul class="list-disc text-lg text-left text-white w-full px-2 z-99 pl-5">
        {#each perks as perk}
          <li>{perk}</li>
        {/each}
      </ul>
    {/if}
    <!-- check if slot or use perks -->
    <div class="pl-5">
      <slot />
    </div>
    <div class="pl-5">
      <slot name="footer" />
    </div>
  </div>
</div>
