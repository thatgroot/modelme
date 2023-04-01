<script lang="ts">
  export let title: string;
  export let subtitle: string;
  export let instruction: string;
  export let perks: string[];
  export let size: "wide" | "tall" = "tall";
</script>

<div
  class="hidden group-hover:flex overflow-hidden right-0 bottom-0 hover:h-full flex-col gap-{size ===
  'wide'
    ? '6'
    : '20'} items-start z-99 p-6 h-full w-full  absolute left-[-1px] top-[-1px] bg-gradient-to-b from-[#4434c9]/80 to-[#4434c9]/40 transition-[height]"
>
  <div class="flex flex-col justify-start items-start relative">
    <p class="text-lg font-semibold text-left text-white">
      {subtitle}
    </p>
    <p class="text-[32px] font-semibold text-left text-white">
      {title}
    </p>
  </div>
  <div class="flex flex-col justify-start items-start relative gap-6">
    {#if instruction}
      <div class="w-[312px] text-lg text-left text-white">
        {instruction}
      </div>
    {/if}

    <ul class="list-disc  text-lg text-left text-white w-full px-2 z-99">
      {#each perks as perk}
        <li>{perk}</li>
      {/each}
    </ul>
  </div>
</div>
