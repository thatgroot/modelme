<script lang="ts">
  import { createEventDispatcher } from "svelte";
  const dispatch = createEventDispatcher();
</script>

<div
  class="z-[999] fixed top-0 left-0 bottom-0 right-0 flex flex-col justify-center items-center gap-6 p-8 bg-[#232323]/50"
>
  <!-- svelte-ignore a11y-click-events-have-key-events -->
  <div
    on:click={() => {
      dispatch("close");
    }}
    class="flex flex-col justify-center items-center  absolute left-0 top-0 right-0 bottom-0 gap-6 p-8 bg-[#232323]/50"
  />
  <slot />
</div>
