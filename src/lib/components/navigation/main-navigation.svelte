<script>
  import { push } from "svelte-spa-router";
  import logo from "../../../assets/logo.png";
  import profile_image from "../../../assets/profile-image.png";
</script>

<div class="bg-white w-full flex justify-between py-8">
  <button
    on:click={() => {
      push("/");
    }}
    class="bg-transparent border-0 flex justify-between items-center gap-4"
  >
    <img
      alt="..."
      src={logo}
      class="w-24  object-cover border-2 border-black p-2"
    />
    <p class="text-[50px] text-left text-neutral-900">MODELME</p>
  </button>

  <div
    class="flex justify-center items-center  py-8 border-t-0 border-r-0 border-b border-l-0 border-[#d9d9d9]"
  >
    <div class="flex justify-start items-start w-6 h-6 gap-8" />
    <div class="flex justify-center items-center w-[890px] relative gap-12">
      <button
        on:click={() => push("/generate")}
        class="text-lg font-medium text-left text-[#9a9a9a]"
      >
        GENERATE
      </button>
      <button
        on:click={() => push("/history")}
        class="text-lg font-medium text-left text-[#9a9a9a]"
      >
        HISTORY
      </button>
    </div>
  </div>

  <div class="flex justify-start items-center   gap-4">
    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <img
      on:click={() => push("/profile")}
      alt="..."
      class="flex-shrink-0"
      src={profile_image}
    />
    <div class="flex flex-col justify-start items-start relative gap-0.5">
      <p class="text-sm font-medium text-left text-[#232323]">Ganteng</p>
      <p class="text-xs text-left text-[#9a9a9a]">ganteng@mail.com</p>
    </div>
  </div>
</div>
