<script lang="ts">
  // Create Folder Download Tag Archive Share Delete

  import Actions from "../navigation/actions.svelte";
  import PageHeader from "../navigation/page-header.svelte";
</script>

<PageHeader title="History">
  <Actions
    on:action={(event) => {
      console.log(event.detail);
    }}
  />
</PageHeader>
