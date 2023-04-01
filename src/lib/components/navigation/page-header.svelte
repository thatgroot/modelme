<script lang="ts">
  export let title: string;
</script>

<div class="flex flex-col gap-6">
  <div class="flex justify-between items-start relative">
    <p class="text-9xl text-left text-[#232323]">{title}</p>
    <slot />
  </div>
  <svg
    height="2"
    viewBox="0 0 1333 2"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
    class="w-full"
    preserveAspectRatio="none"
  >
    <line x1="0.000375094" y1="0.5" x2="1333" y2="1.5" stroke="black"></line>
  </svg>
</div>

