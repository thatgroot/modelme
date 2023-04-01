<script>
  import Actions from "../navigation/actions.svelte";
  import logout_svg from "../../../assets/icons/profile/logout.svg";
  import PageHeader from "../navigation/page-header.svelte";

</script>

<PageHeader title="Profile">
  <Actions
    on:action={(event) => {
      console.log(event.detail);
    }}
    on:sub_action={(event) => {
      console.log(event.detail);
    }}
    actions={[
      // Generate, Team, FAQs
      {
        name: "Generate",
        active: true,
        actions: [
          {
            name: "Logout",
            icon: logout_svg,
            id: "logout",
            text: "danger",
          },
        ],
      },
      {
        name: "Team",
        active: false,
        actions: [
          {
            name: "Logout",
            icon: logout_svg,
            id: "logout",
            text: "danger",
          },
        ],
      },
      {
        name: "FAQs",
        active: false,
        actions: [
          {
            name: "Logout",
            icon: logout_svg,
            id: "logout",
            text: "danger",
          },
        ],
      },
    ]}
  />
</PageHeader>
