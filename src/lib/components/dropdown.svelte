<script lang="ts">
  import { onMount } from "svelte";
  export let command: string;
  export let before: string = "";
  export let after: string = "";
  export let text: string;
  export let show: boolean = false;
  import close_svg from "../../assets/icons/close.svg";
  let show_dropdown = false;
  // toggle dropdown
  function toggle_dropdown() {
    show_dropdown = !show_dropdown;
  }

  onMount(() => {
    show_dropdown = show;
  });
</script>

<div class="relative group">
  <!-- svelte-ignore a11y-click-events-have-key-events -->
  <div
    class="flex justify-center items-center relative gap-2 p-3 cursor-pointer"
    on:click={toggle_dropdown}
  >
    <span class="text-base font-medium text-left text-[#9a9a9a]">
      {command}:
    </span>
    <div
      class="flex justify-center items-center relative gap-2 p-3 border border-[#1f206c]"
    >
      {#if before}
        <img src={before} alt="before" class="h-[18px] relative" />
      {/if}
      <span class="text-base font-medium text-left text-[#232323]">{text}</span>
      {#if after}
        <img src={after} alt="after" class="h-[18px] relative" />
      {/if}
    </div>
  </div>
  <div
    class="{show_dropdown
      ? 'flex'
      : 'hidden'} absolute right-0 flex-col justify-start items-start w-[293px] z-[999] gap-4 p-4 bg-white border border-[#d9d9d9]"
    style="box-shadow: 4px 4px 44px 0 rgba(0,0,0,0.08);"
  >
    <div
      class="flex relative flex-shrink-0 flex-grow-0 items-center justify-between self-stretch"
    >
      <span
        class="flex-shrink-0 flex-grow-0 text-left text-base font-medium text-[#232323]"
      >
        {command}
      </span>
      <!-- close svg -->
      <button class="bg-transparent p-0 border-0" on:click={toggle_dropdown}>
        <img src={close_svg} alt="close" class="h-[18px] relative" />
      </button>
    </div>
    <slot />
  </div>
</div>
