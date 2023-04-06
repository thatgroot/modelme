<script lang="ts">
  import Checkbox from "../checkbox.svelte";
  import Dropdown from "../dropdown.svelte";
  import Input from "../input.svelte";
  import Radio from "../radio.svelte";
  import grid_svg from "../../../assets/icons/grid.svg";
  import arrow_head_down from "../../../assets/icons/arrow-head-down.svg";
  import arrow_up from "../../../assets/icons/arrow-up.svg";
  import list_svg from "../../../assets/icons/list.svg";
  import column_svg from "../../../assets/icons/column.svg";
  import close_svg from "../../../assets/icons/close-white.svg";
  import RangeSlider from "../range-slider.svelte";
  let show_tags: boolean = false;
  let show_tags_drop_down: boolean = false;
</script>

<div class="flex items-center justify-between gap-4">
  <Input placeholder="Search..." />

  <div class="flex flex-grow justify-between items-center relative">
    <div class="flex justify-start items-center relative gap-2">
      <Checkbox label="Select all" />
    </div>
    <div class="flex justify-start items-center relative gap-4">
      <!-- "Kind", "Date Created", "Name" -->
      <Dropdown
        command="Sort by"
        before={arrow_up}
        after={arrow_head_down}
        text="Folders"
      >
        <Radio label="Kind" name="sort" value="kind" checked={true} />
        <Radio label="Date Created" name="sort" value="date" checked={false} />
        <Radio label="Name" name="sort" value="name" checked={false} />
      </Dropdown>
      <Dropdown
        command="Filter by"
        before={arrow_up}
        after={arrow_head_down}
        text="Tag"
      >
        <Radio
          label="Tag"
          name="filter"
          value="tag"
          on:change={(e) => {
            show_tags = e.detail;
          }}
        />

        <Radio
          label="License"
          name="filter"
          value="license"
          checked={false}
          on:change={(e) => {
            show_tags = false;
          }}
        />

        <div
          class="flex flex-col justify-start items-start gap-3 z-[9999] absolute left-[102%] top-0 w-max {show_tags
            ? 'block'
            : 'hidden'}"
        >
          <div
            class="flex flex-col justify-start items-start relative gap-[22px] bg-white p-[14px] border-[1px] border-[#626398]"
          >
            <input
              class="outline-none appearance-none text-[11] font-medium text-left text-[#9a9a9a] bg-transparent"
              placeholder="Enter any value..."
            />
            <div
              class="flex justify-start items-start gap-[11px]"
            >
              {#each ["foo", "bar", "fizz", "buzz"] as title}
                <div
                  class="flex rounded-[4px] gap-3 items-center justify-center px-3 py-2 relative bg-[#1f206c]"
                >
                  <span
                    class="text-[11px] font-medium text-left text-white"
                  >
                    {title}
                  </span>
                  <img src={close_svg} alt="..." />
                  <!-- close -->
                </div>
              {/each}
            </div>
          </div>
          <div
            class="flex justify-start items-start relative gap-[9px] px-[7px] py-[2px] rounded-[5px] bg-[#f4f4f4]"
          >
            <span
              class="text-[11.087718963623047px] font-medium text-left text-[#1f206c]"
            >
              foo, bar, fizz, buzz
            </span>
          </div>
        </div>
      </Dropdown>

      <Dropdown
        command="View:"
        before={grid_svg}
        after={arrow_head_down}
        text="Grid"
      >
        <Radio label="Grid" name="view" icon={grid_svg} />
        <Radio label="List" name="view" icon={list_svg} />
        <Radio label="Column" name="view" icon={column_svg} />
        <RangeSlider min={0} max={12} />
      </Dropdown>
    </div>
  </div>
</div>
