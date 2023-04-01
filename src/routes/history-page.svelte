<script lang="ts">
  import HistoryItem from "../lib/components/history/history-item.svelte";
  import HistoryNavigation from "../lib/components/history/history-navigation.svelte";
  import HistoryModal from "../lib/components/history/history-modal.svelte";
  import image_1 from "../assets/1.png";
  import image_2 from "../assets/2.png";
  import image_3 from "../assets/3.png";
  import image_4 from "../assets/4.png";
  import image_5 from "../assets/5.png";
  import image_6 from "../assets/6.png";
  import image_7 from "../assets/7.png";
  import image_8 from "../assets/8.png";
  import image_9 from "../assets/9.png";
  import image_10 from "../assets/10.png";
  import image_11 from "../assets/11.png";
  import image_12 from "../assets/12.png";
  import image_13 from "../assets/13.png";
  import HistoryFilters from "../lib/components/history/history-filters.svelte";
  const image_items = [
    [
      [image_1, image_2, image_3],
      [image_4, image_5, image_6],
      [image_7, image_8, image_9],
      [image_10, image_11, image_12, image_13],
    ],
    [
      [image_1, image_2, image_3],
      [image_4, image_5, image_6],
      [image_7, image_8, image_9],
      [image_10, image_11, image_12, image_13],
    ],
  ];

  let show_modal: boolean = false;
</script>

<div id="history-section" class="flex flex-col gap-6">
  <!-- toggle modal -->
  {#if show_modal}
    <HistoryModal
      on:close={(event) => {
        show_modal = false;
      }}
    />
  {/if}
  <div class="flex flex-col gap-6">
    <HistoryNavigation />
    <HistoryFilters />
  </div>

  <div class="flex flex-col gap-4">
    {#each image_items as set}
      <div class="flex w-full z-10 justify-between">
        {#each set as items}
          <HistoryItem
            on:imageclick={(event) => {
              show_modal = true;
            }}
            images={items}
            title="History Item 1"
            author="Author 1"
            alt="Alt 1"
            tags={["tag1", "tag2", "tag3"]}
          />
        {/each}
      </div>
    {/each}
  </div>
</div>
