<script lang="ts">
  import { createEventDispatcher } from "svelte";

  export let label: string = "";
  export let name: string = "";
  export let size: "small" | "default" = "default";
  export let border: "border-[#9a9a9a]" | "border-[#ffffff]" =
    "border-[#9a9a9a]";
  const dispatch = createEventDispatcher();
</script>

<div class="flex items-center">
  <input
    type="checkbox"
    {name}
    value="yes"
    on:change={(e) => {
      // @ts-ignore
      dispatch("change", e.target.checked);
    }}
    class="opacity-0 absolute {size === 'small'
      ? 'h-4 w-4'
      : 'h-6 w-6'} cursor-pointer}"
  />
  <div
    class="bg-transprent border-2 rounded-md {border} h-4 w-4 flex flex-shrink-0 justify-center items-center mr-2 focus-within:{border}"
  >
    <svg
      width="16"
      height="16"
      viewBox="0 0 15 16"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
      preserveAspectRatio="none"
    >
      <path
        d="M10.6425 0.5H4.3575C1.6275 0.5 0 2.1275 0 4.8575V11.135C0 13.8725 1.6275 15.5 4.3575 15.5H10.635C13.365 15.5 14.9925 13.8725 14.9925 11.1425V4.8575C15 2.1275 13.3725 0.5 10.6425 0.5ZM11.085 6.275L6.8325 10.5275C6.7275 10.6325 6.585 10.6925 6.435 10.6925C6.285 10.6925 6.1425 10.6325 6.0375 10.5275L3.915 8.405C3.6975 8.1875 3.6975 7.8275 3.915 7.61C4.1325 7.3925 4.4925 7.3925 4.71 7.61L6.435 9.335L10.29 5.48C10.5075 5.2625 10.8675 5.2625 11.085 5.48C11.3025 5.6975 11.3025 6.05 11.085 6.275Z"
        fill="#0085FF"
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
