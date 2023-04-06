<script lang="ts">
  export let placeholder: string;
  export let width: string = "w-[366px]";
  export let type: string = "text";
  export let name: string = "";
  export let id: string = "";
  export let value: string = "";
</script>

<div
  class="flex flex-col justify-center items-center {width} relative bg-white border border-[#1f206c]"
>
  <input
    {type}
    {name}
    {id}
    {value}
    class="self-stretch w-[334px] text-lg font-medium text-left text-[#232323] outline-none  p-4"
    {placeholder}
  />
</div>
