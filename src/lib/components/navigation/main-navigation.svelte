<script>
  import { push } from "svelte-spa-router";
  import logo from "../../../assets/logo.png";
  import profile_image from "../../../assets/profile-image.png";
</script>

<div
  class="bg-white w-full flex justify-between py-0 border-t-0 border-r-0 border-b border-l-0 border-[#d9d9d9]"
>
  <button
    on:click={() => {
      push("/");
    }}
    class="bg-transparent border-0 flex justify-between items-center gap-4"
  >
    <img
      alt="..."
      src={logo}
      class="w-24 object-cover border-2 border-black p-2"
    />
    <p
      class="text-[50px] text-left text-neutral-900 font-[var(--theme-font-family-heading)]"
    >
      MODELME
    </p>
  </button>

  <div class="flex justify-center items-center py-8">
    <div class="flex justify-start items-start w-6 h-6 gap-8" />
    <div class="flex justify-center items-center relative gap-12">
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

  <div class="flex gap-6 items-center">
    <div
      class="flex justify-center items-center flex-grow-0 flex-shrink-0 relative gap-2"
    >
      <div
        class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-1.5"
      >
        <svg
          width="18"
          height="18"
          viewBox="0 0 18 18"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          class="flex-grow-0 flex-shrink-0 w-[18px] h-[18px] relative"
          preserveAspectRatio="xMidYMid meet"
        >
          <path
            d="M9.5625 11.9402H10.05C10.5375 11.9402 10.9425 11.5052 10.9425 10.9802C10.9425 10.3277 10.71 10.2002 10.3275 10.0652L9.57 9.80273V11.9402H9.5625Z"
            fill="#1F206C"
          />
          <path
            d="M8.97755 1.42482C4.83755 1.43982 1.48505 4.80732 1.50005 8.94732C1.51505 13.0873 4.88255 16.4398 9.02255 16.4248C13.1625 16.4098 16.515 13.0423 16.5 8.90232C16.4851 4.76232 13.1175 1.41732 8.97755 1.42482ZM10.6951 8.99982C11.2801 9.20232 12.0676 9.63732 12.0676 10.9798C12.0676 12.1348 11.16 13.0648 10.05 13.0648H9.56255V13.4998C9.56255 13.8073 9.30755 14.0623 9.00005 14.0623C8.69255 14.0623 8.43755 13.8073 8.43755 13.4998V13.0648H8.16755C6.93755 13.0648 5.94005 12.0298 5.94005 10.7548C5.94005 10.4473 6.19505 10.1923 6.50255 10.1923C6.81005 10.1923 7.06505 10.4473 7.06505 10.7548C7.06505 11.4073 7.56005 11.9398 8.16755 11.9398H8.43755V9.40482L7.30505 8.99982C6.72005 8.79732 5.93255 8.36232 5.93255 7.01982C5.93255 5.86482 6.84005 4.93482 7.95005 4.93482H8.43755V4.49982C8.43755 4.19232 8.69255 3.93732 9.00005 3.93732C9.30755 3.93732 9.56255 4.19232 9.56255 4.49982V4.93482H9.83255C11.0625 4.93482 12.0601 5.96982 12.0601 7.24482C12.0601 7.55232 11.805 7.80732 11.4976 7.80732C11.1901 7.80732 10.9351 7.55232 10.9351 7.24482C10.9351 6.59232 10.4401 6.05982 9.83255 6.05982H9.56255V8.59482L10.6951 8.99982Z"
            fill="#1F206C"
          />
          <path
            d="M7.06445 7.02756C7.06445 7.68006 7.29695 7.80756 7.67945 7.94256L8.43695 8.20506V6.06006H7.94945C7.46195 6.06006 7.06445 6.49506 7.06445 7.02756Z"
            fill="#1F206C"
          />
        </svg>
        <span class="flex-grow-0 flex-shrink-0 text-sm text-left text-[#232323]">
          Balance:
        </span>
      </div>
      <span
        class="flex-grow-0 flex-shrink-0 text-base font-semibold text-left text-[#232323]"
      >
        1,200 credits
      </span>
    </div>

    <div class="flex justify-start items-center gap-4">
      <!-- svelte-ignore a11y-click-events-have-key-events -->
      <img
        on:click={() => push("/profile")}
        alt="..."
        class="flex-shrink-0"
        src={profile_image}
      />
      <div class="flex flex-col justify-start items-start relative gap-0.5">
        <span class="text-sm font-medium text-left text-[#232323]">Ganteng</span
        >
        <span class="text-xs text-left text-[#9a9a9a]">ganteng@mail.com</span>
      </div>
    </div>
  </div>
</div>
