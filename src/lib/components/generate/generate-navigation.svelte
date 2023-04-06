<script>
  import Actions from "../navigation/actions.svelte";
  import delete_icon from "../../../assets/icons/history/delete.svg";
  import PageHeader from "../navigation/page-header.svelte";
</script>

<PageHeader title="Generate">
  <Actions
    actions={[
      {
        name: "Balance: 100",
        active: true,
        actions: [
          {
            name: "Delete",
            icon: delete_icon,
            id: "delete",
            text: "danger",
          },
        ],
      },
    ]}
    on:action={(event) => {
      console.log(event.detail);
    }}
  />
</PageHeader>
