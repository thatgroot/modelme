<script lang="ts">
  import { createEventDispatcher } from "svelte";
  import logout_svg from "../assets/icons/profile/logout.svg";
  import Actions from "../lib/components/navigation/actions.svelte";
  import MainNavigation from "../lib/components/navigation/main-navigation.svelte";
  import PageHeader from "../lib/components/navigation/page-header.svelte";
  import ProfileNavigation from "../lib/components/profile/profile-navigation.svelte";
  import ProfileFaqs from "../lib/components/profile/sections/profile-faqs.svelte";
  import ProfileGeneral from "../lib/components/profile/sections/profile-general.svelte";
  import ProfilePayment from "../lib/components/profile/sections/profile-payment.svelte";
  import ProfileTeam from "../lib/components/profile/sections/profile-team.svelte";
  import PageWrapper from "../lib/components/page-wrapper.svelte";
  let subscriptions: Array<{
    title: string;
    pricing: {
      period: "mo" | "yr";
      currency: string | "€" | "$";
      amount: number;
    }[];
    subtitle: string;
    perks: Array<string>;
  }> = [
    {
      title: "High Grade (HG)",
      pricing: [
        {
          period: "mo",
          currency: "€",
          amount: 30,
        },
        {
          period: "yr",
          currency: "€",
          amount: 288,
        },
      ],
      subtitle: "Save 20% on yearly plans",
      perks: [
        "3,000 fast generations per month.",
        "Unlimited slow generations.",
        "3 parallel fast generations.",
        "Commercial license.",
        "Images are public.",
      ],
    },
    {
      title: "Real Grade (RG)",
      subtitle: "Unlimited slow generations.",
      pricing: [
        {
          period: "mo",
          currency: "€",
          amount: 48,
        },
        {
          period: "yr",
          currency: "€",
          amount: 576,
        },
      ],
      perks: [
        "Unlimited slow generations.",
        "3 parallel fast generations.",
        "Commercial license.",
        "Keep images private.",
        "7,000 fast generations per month.",
      ],
    },
    {
      title: "Entry Grade (EG)",
      perks: [
        "No slow generations",
        "2 parallel fast generations.",
        "Commercial license (solo).",
        "Images are public.",
        "1,000 fast generations per month.",
      ],
      subtitle: "Save 20% on yearly plans",
      pricing: [
        {
          period: "mo",
          currency: "€",
          amount: 10,
        },
        {
          period: "yr",
          currency: "€",
          amount: 96,
        },
      ],
    },
  ];
  const dispatch = createEventDispatcher();

  let current_action: "general" | "team" | "faqs" | "" = "";
</script>

<PageWrapper>
  <MainNavigation />
  <div id="generate-section" class="flex flex-col gap-6">
    <div class="flex flex-col gap-6 mt-4">
      <PageHeader title="Profile">
        <Actions
          on:action={(event) => {
            current_action = event.detail;
          }}
          on:sub_action={(event) => {
            //
          }}
          actions={[
            // Generate, Team, FAQs
            {
              name: "General",
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
    </div>
    {#if current_action === ""}
      <ProfilePayment />
    {:else if current_action === "general"}
      <ProfileGeneral {subscriptions} />
    {:else if current_action === "team"}
      <ProfileTeam />
    {:else if current_action === "faqs"}
      <ProfileFaqs />
    {:else}
      <h1>...</h1>
    {/if}

    <!-- profile general -->
  </div>
</PageWrapper>
