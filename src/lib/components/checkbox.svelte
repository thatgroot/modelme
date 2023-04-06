<script lang="ts">
  import { createEventDispatcher } from "svelte";

  export let label: string = "";
  export let name: string = "";
  export let size: "small" | "default" = "default";
  export let border: "border-[#9a9a9a]" | "border-[#ffffff]" =
    "border-[#9a9a9a]";
    const dispatch = createEventDispatcher()
</script>

<div class="flex items-center">
  <input
    type="checkbox"
    {name}
    value="yes"
    on:change={(e)=>{
      // @ts-ignore
      dispatch('change',e.target.checked)
    }}
    class="opacity-0 absolute {size === 'small'
      ? 'h-4 w-4'
      : 'h-6 w-6'} cursor-pointer}"
  />
  <div
    class="bg-transprent border-2 rounded-md {border} {size === 'small'
      ? 'h-4 w-4'
      : 'h-6 w-6'} flex flex-shrink-0 justify-center items-center mr-2 focus-within:{border}"
  >
    <svg
      width="24"
      height="24"
      viewBox="0 0 24 24"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path
        d="M16.19 2H7.81C4.17 2 2 4.17 2 7.81V16.18C2 19.83 4.17 22 7.81 22H16.18C19.82 22 21.99 19.83 21.99 16.19V7.81C22 4.17 19.83 2 16.19 2ZM16.78 9.7L11.11 15.37C10.97 15.51 10.78 15.59 10.58 15.59C10.38 15.59 10.19 15.51 10.05 15.37L7.22 12.54C6.93 12.25 6.93 11.77 7.22 11.48C7.51 11.19 7.99 11.19 8.28 11.48L10.58 13.78L15.72 8.64C16.01 8.35 16.49 8.35 16.78 8.64C17.07 8.93 17.07 9.4 16.78 9.7Z"
        fill={border === "border-[#9a9a9a]" ? "#aeaeae" : "white"}
      />
    </svg>
  </div>
  <!-- if lable is empty -->
  {#if label !== ""}
    <label
      for="A3-yes"
      class="select-none text-base font-medium text-left text-[#9a9a9a]"
      >{label}</label
    >
  {/if}
</div>

<style>
  input + div svg {
    @apply hidden;
  }
  input:checked + div {
    @apply border-0;
  }
  input:checked + div svg {
    @apply block;
  }
</style>
