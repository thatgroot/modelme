<script>
  import Checkbox from "../checkbox.svelte";
  import Input from "../input.svelte";
</script>

<div class="flex  items-center w-fit gap-4">
  <Input placeholder="Search..." />

  <div
    class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-2"
  >
    <Checkbox label={"Select all"} />
  </div>
</div>
