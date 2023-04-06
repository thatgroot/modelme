<script>
  import { push } from "svelte-spa-router";
  import logo from "../../../assets/logo.png";
</script>

<div
  class="flex justify-between items-center  py-4 border-t-0 border-r-0 border-b border-l-0 border-[#232323]/[0.16] px-12"
>
  <div
    class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-3"
  >
    <div class="flex-grow-0 flex-shrink-0 w-[97px] h-[65.15px]">
      <button
        class="bg-transparent border-0 flex items-center justify-center"
        on:click={() => {
          push("/");
        }}
      >
        <img
          src={logo}
          alt="..."
          class="w-[82.52px] h-[52.12px] absolute left-[6.74px] top-[6.74px] object-cover"
        />
      </button>
      <div
        class="w-[97px] h-[65.15px] absolute left-[-0.5px] top-[-0.5px] bg-transparent border border-black"
      />
    </div>
    <p
      class="text-[50px] text-left text-neutral-900"
    >
      MODELME
    </p>
  </div>
  <div
    class="flex justify-start items-start flex-grow-0 flex-shrink-0 relative gap-12"
  >
    <a
      href="#howto"
      class="flex-grow-0 flex-shrink-0 text-lg font-medium text-left text-black"
    >
      HOW TO
    </a>
    <a
      href="#gallery"
      class="flex-grow-0 flex-shrink-0 text-lg font-medium text-left text-black"
    >
      GALLERY
    </a>
    <a
      href="#pricing"
      class="flex-grow-0 flex-shrink-0 text-lg font-medium text-left text-black"
    >
      PRICING
    </a>
    <a
      href="#team"
      class="flex-grow-0 flex-shrink-0 text-lg font-medium text-left text-black"
    >
      TEAM
    </a>
    <a
      href="#contact"
      class="flex-grow-0 flex-shrink-0 text-lg font-medium text-left text-black"
    >
      CONTACT
    </a>
  </div>
  <div
    class="flex justify-start items-start flex-grow-0 flex-shrink-0 relative gap-8"
  >
    <button
      class="bg-transparent border-0"
      on:click={() => {
        push("/profile");
      }}
    >
      <svg
        width="24"
        height="25"
        viewBox="0 0 24 25"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        class="flex-grow-0 flex-shrink-0 w-6 h-6 relative"
        preserveAspectRatio="none"
      >
        <path
          d="M22 12.5747C22 7.06471 17.51 2.57471 12 2.57471C6.49 2.57471 2 7.06471 2 12.5747C2 15.4747 3.25 18.0847 5.23 19.9147C5.23 19.9247 5.23 19.9247 5.22 19.9347C5.32 20.0347 5.44 20.1147 5.54 20.2047C5.6 20.2547 5.65 20.3047 5.71 20.3447C5.89 20.4947 6.09 20.6347 6.28 20.7747C6.35 20.8247 6.41 20.8647 6.48 20.9147C6.67 21.0447 6.87 21.1647 7.08 21.2747C7.15 21.3147 7.23 21.3647 7.3 21.4047C7.5 21.5147 7.71 21.6147 7.93 21.7047C8.01 21.7447 8.09 21.7847 8.17 21.8147C8.39 21.9047 8.61 21.9847 8.83 22.0547C8.91 22.0847 8.99 22.1147 9.07 22.1347C9.31 22.2047 9.55 22.2647 9.79 22.3247C9.86 22.3447 9.93 22.3647 10.01 22.3747C10.29 22.4347 10.57 22.4747 10.86 22.5047C10.9 22.5047 10.94 22.5147 10.98 22.5247C11.32 22.5547 11.66 22.5747 12 22.5747C12.34 22.5747 12.68 22.5547 13.01 22.5247C13.05 22.5247 13.09 22.5147 13.13 22.5047C13.42 22.4747 13.7 22.4347 13.98 22.3747C14.05 22.3647 14.12 22.3347 14.2 22.3247C14.44 22.2647 14.69 22.2147 14.92 22.1347C15 22.1047 15.08 22.0747 15.16 22.0547C15.38 21.9747 15.61 21.9047 15.82 21.8147C15.9 21.7847 15.98 21.7447 16.06 21.7047C16.27 21.6147 16.48 21.5147 16.69 21.4047C16.77 21.3647 16.84 21.3147 16.91 21.2747C17.11 21.1547 17.31 21.0447 17.51 20.9147C17.58 20.8747 17.64 20.8247 17.71 20.7747C17.91 20.6347 18.1 20.4947 18.28 20.3447C18.34 20.2947 18.39 20.2447 18.45 20.2047C18.56 20.1147 18.67 20.0247 18.77 19.9347C18.77 19.9247 18.77 19.9247 18.76 19.9147C20.75 18.0847 22 15.4747 22 12.5747ZM16.94 17.5447C14.23 15.7247 9.79 15.7247 7.06 17.5447C6.62 17.8347 6.26 18.1747 5.96 18.5447C4.44 17.0047 3.5 14.8947 3.5 12.5747C3.5 7.88471 7.31 4.07471 12 4.07471C16.69 4.07471 20.5 7.88471 20.5 12.5747C20.5 14.8947 19.56 17.0047 18.04 18.5447C17.75 18.1747 17.38 17.8347 16.94 17.5447Z"
          fill="#1F206C"
        />
        <path
          d="M12 7.50488C9.93 7.50488 8.25 9.18488 8.25 11.2549C8.25 13.2849 9.84 14.9349 11.95 14.9949C11.98 14.9949 12.02 14.9949 12.04 14.9949C12.06 14.9949 12.09 14.9949 12.11 14.9949C12.12 14.9949 12.13 14.9949 12.13 14.9949C14.15 14.9249 15.74 13.2849 15.75 11.2549C15.75 9.18488 14.07 7.50488 12 7.50488Z"
          fill="#1F206C"
        />
      </svg>
    </button>
  </div>
</div>
