<script lang="ts">
  import { createEventDispatcher } from "svelte";

  export let label: string = "";
  export let icon: string = "";
  export let name: string = "";
  export let checked: boolean = false;
  export let value: string = "";
  export let id: string = "";
  export let white: boolean = false;
  // create dispatch
  const dispatch = createEventDispatcher();
  export let border: "border-[#d9d9d9]" | "border-[#ffffff]" =
    "border-[#d9d9d9]";
</script>

<div class="flex relative items-center justify-start gap-2 self-stretch py-2">
  <div class="flex items-center">
    <input
      type="radio"
      {id}
      {name}
      {value}
      {checked}
      on:change={(e) => {
        // @ts-ignore
        dispatch("change", e.target.checked);
      }}
      class="opacity-0 absolute h-5 w-5 cursor-pointer"
    />
    <div
      class="bg-transprent {white
        ? 'border-[1px]'
        : 'border-[3px]'}  rounded-full {border} h-5 w-5 flex flex-shrink-0 justify-center items-center mr-2 focus-within:border-{border}"
    >
      {#if white}
        <svg
          width="16"
          height="15"
          viewBox="0 0 16 15"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M8.33398 0C4.20148 0 0.833984 3.3675 0.833984 7.5C0.833984 11.6325 4.20148 15 8.33398 15C12.4665 15 15.834 11.6325 15.834 7.5C15.834 3.3675 12.4665 0 8.33398 0ZM11.919 5.775L7.66648 10.0275C7.56148 10.1325 7.41898 10.1925 7.26898 10.1925C7.11898 10.1925 6.97648 10.1325 6.87148 10.0275L4.74898 7.905C4.53148 7.6875 4.53148 7.3275 4.74898 7.11C4.96648 6.8925 5.32648 6.8925 5.54398 7.11L7.26898 8.835L11.124 4.98C11.3415 4.7625 11.7015 4.7625 11.919 4.98C12.1365 5.1975 12.1365 5.55 11.919 5.775Z"
            fill="white"
          />
        </svg>
      {:else}
        <svg
          width="20"
          height="20"
          viewBox="0 0 20 20"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          class=""
        >
          <circle cx="10" cy="10" r="6" fill="#1F206C" class="" />
          <rect
            x="1"
            y="1"
            width="18"
            height="18"
            rx="9"
            stroke="#1F206C"
            stroke-width="2"
            class=""
          />
        </svg>
      {/if}
    </div>
  </div>
  <!--<Radio>-->
  <!-- if icon  -->
  {#if icon}
    <img src={icon} alt="label icon" class="h-[18px] relative" />
  {/if}
  <span class="text-left text-base font-medium text-[#232323]">{label} </span>
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
