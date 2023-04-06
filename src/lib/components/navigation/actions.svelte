<script lang="ts">
  import create_folder from "../../../assets/icons/history/create-folder.svg";
  import download from "../../../assets/icons/history/download.svg";
  import tag from "../../../assets/icons/history/tag.svg";
  import archive from "../../../assets/icons/history/archive.svg";
  import share from "../../../assets/icons/history/share.svg";
  import divider_svg from "../../../assets/icons/divider.svg";

  import delete_icon from "../../../assets/icons/history/delete.svg";
  // restore
  import restore from "../../../assets/icons/history/restore.svg";
  import { createEventDispatcher, onMount } from "svelte";

  let active_action: {
    name: string;
    active: boolean;
    actions: {
      name: string;
      icon: string;
      id: string;
      text?: "normal" | "danger";
    }[];
  };

  export let actions: Array<{
    name: string;
    active: boolean;
    actions: {
      name: string;
      icon: string;
      id: string;
      text?: "normal" | "danger";
    }[];
  }> = [
    {
      name: "History",
      active: true,
      actions: [
        {
          name: "Create Folder",
          icon: create_folder,
          id: "create_folder",
        },
        {
          name: "Download",
          icon: download,
          id: "download",
        },
        {
          name: "Tag",
          icon: tag,
          id: "tag",
        },
        {
          name: "Archive",
          icon: archive,
          id: "archive",
        },
        {
          name: "Share",
          icon: share,
          id: "share",
        },
        {
          name: "Delete",
          icon: delete_icon,
          id: "delete",
        },
      ],
    },
    {
      name: "Archive",
      active: false,
      actions: [
        {
          name: "Create Folder",
          icon: create_folder,
          id: "create_folder",
        },
        {
          name: "Download",
          icon: download,
          id: "download",
        },
        {
          name: "Tag",
          icon: tag,
          id: "tag",
        },
        {
          name: "Share",
          icon: share,
          id: "share",
        },
        {
          name: "Delete",
          icon: delete_icon,
          id: "delete",
        },
      ],
    },
    {
      name: "Trash",
      active: false,
      actions: [
        {
          name: "Restore",
          icon: restore,
          id: "restore",
        },
        {
          name: "Permanently Delete",
          icon: delete_icon,
          id: "delete",
        },
      ],
    },
  ];
  const dispatch = createEventDispatcher();

  onMount(() => {
    active_action = actions[0];
  });
</script>

<div class="flex flex-col items-end gap-8">
  <div class="flex justify-start items-end gap-[9.67px]">
    {#each actions as action}
      <div
        class="flex justify-center items-center w-20 relative p-3 bg-white border-t-0 border-r-0 {action.active
          ? 'border-b-[3px]'
          : 'border-b'} border-l-0 border-[#1f206c]"
      >
        <button
          on:click={() => {
            // change active status
            actions.forEach((a) => {
              a.active = false;
            });
            action.active = true;
            active_action = action;
            dispatch("action", action.name.toLowerCase().replaceAll(" ", "_"));
          }}
          class="flex-grow-0 flex-shrink-0 text-sm font-medium text-center text-[#232323]"
        >
          {action.name}
        </button>
      </div>
    {/each}
  </div>

  <div class="gap-x-[5px] flex">
    {#if active_action}
      {#each active_action.actions as { name, icon, id, text }, i}
        <button
          on:click={() => {
            dispatch("sub_action", id);
          }}
          class="flex justify-start py-2 px-3 w-max items-center relative gap-2"
        >
          <img src={icon} alt={name} />
          <span
            class="text-base font-medium flex-grow text-left {text === 'danger'
              ? 'text-[#eb5842]'
              : 'text-[#232323]'}"
          >
            {name}
          </span>
        </button>
        {#if i < active_action.actions.length-1}
          <img src={divider_svg} alt="..." />
        {/if}
      {/each}
    {/if}
  </div>
</div>
