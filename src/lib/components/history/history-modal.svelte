<script lang="ts">
  import { createEventDispatcher } from "svelte";
  import image_14 from "../../../assets/14.png";
  const dispatch = createEventDispatcher();
</script>

<!-- svelte-ignore a11y-click-events-have-key-events -->
<div
  on:click={() => {
    dispatch("close");
  }}
  class="z-[999] fixed top-0 left-0 bottom-0 right-0 flex flex-col justify-center items-center gap-6 p-8 bg-[#232323]/50"
>
  <div class="flex-grow-0 flex-shrink-0 w-[1010px] h-[814px] relative">
    <svg
      width="1010"
      height="789"
      viewBox="0 0 1010 789"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
      class="absolute left-[-1px] top-6"
      preserveAspectRatio="none"
    >
      <path d="M0 0H1010V789H0V0Z" fill="white" /></svg
    ><img
      alt=".."
      src={image_14}
      class="w-[483px] h-[645px] absolute left-[467px] top-[65px] object-cover"
    />
    <div
      class="flex justify-center items-center h-[72px] absolute left-[464px] top-[711px] py-4 bg-white"
    >
      <div
        class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-2 px-3 py-2"
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
            d="M6.99023 8.76001L8.91023 10.68L10.8302 8.76001"
            stroke="#232323"
            stroke-width="1.5"
            stroke-miterlimit="10"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M8.91016 3V10.6275"
            stroke="#232323"
            stroke-width="1.5"
            stroke-miterlimit="10"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M15 9.13501C15 12.45 12.75 15.135 9 15.135C5.25 15.135 3 12.45 3 9.13501"
            stroke="#232323"
            stroke-width="1.5"
            stroke-miterlimit="10"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>
        <p
          class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-[#232323]"
        >
          Download
        </p>
      </div>
      <svg
        width="2"
        height="40"
        viewBox="0 0 2 40"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        class="self-stretch flex-grow-0 flex-shrink-0"
        preserveAspectRatio="none"
      >
        <path d="M1 0V40" stroke="#D9D9D9" />
      </svg>
      <div
        class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-2 px-3 py-2 bg-white"
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
            d="M3.12779 11.4751L6.52529 14.8726C7.92029 16.2676 10.1853 16.2676 11.5878 14.8726L14.8803 11.5801C16.2753 10.1851 16.2753 7.9201 14.8803 6.5176L11.4753 3.1276C10.7628 2.4151 9.78029 2.0326 8.77529 2.0851L5.02529 2.2651C3.52529 2.3326 2.33279 3.5251 2.25779 5.0176L2.07779 8.7676C2.03279 9.7801 2.41529 10.7626 3.12779 11.4751Z"
            stroke="#232323"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M7.125 9C8.16053 9 9 8.16053 9 7.125C9 6.08947 8.16053 5.25 7.125 5.25C6.08947 5.25 5.25 6.08947 5.25 7.125C5.25 8.16053 6.08947 9 7.125 9Z"
            stroke="#232323"
            stroke-width="1.5"
            stroke-linecap="round"
          />
        </svg>
        <p
          class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-[#232323]"
        >
          Tag
        </p>
      </div>
      <svg
        width="2"
        height="40"
        viewBox="0 0 2 40"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        class="self-stretch flex-grow-0 flex-shrink-0"
        preserveAspectRatio="none"
      >
        <path d="M1 0V40" stroke="#D9D9D9" />
      </svg>
      <div
        class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-2 px-3 py-2"
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
            d="M6.9375 6.7876C8.2725 7.2751 9.7275 7.2751 11.0625 6.7876"
            stroke="#232323"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M12.6152 1.5H5.38523C3.78773 1.5 2.49023 2.805 2.49023 4.395V14.9625C2.49023 16.3125 3.45773 16.8825 4.64273 16.23L8.30273 14.1975C8.69273 13.98 9.32273 13.98 9.70523 14.1975L13.3652 16.23C14.5502 16.89 15.5177 16.32 15.5177 14.9625V4.395C15.5102 2.805 14.2127 1.5 12.6152 1.5Z"
            stroke="#232323"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M12.6152 1.5H5.38523C3.78773 1.5 2.49023 2.805 2.49023 4.395V14.9625C2.49023 16.3125 3.45773 16.8825 4.64273 16.23L8.30273 14.1975C8.69273 13.98 9.32273 13.98 9.70523 14.1975L13.3652 16.23C14.5502 16.89 15.5177 16.32 15.5177 14.9625V4.395C15.5102 2.805 14.2127 1.5 12.6152 1.5Z"
            stroke="#232323"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>
        <p
          class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-[#232323]"
        >
          Archive
        </p>
      </div>
      <svg
        width="2"
        height="40"
        viewBox="0 0 2 40"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        class="self-stretch flex-grow-0 flex-shrink-0"
        preserveAspectRatio="none"
      >
        <path d="M1 0V40" stroke="#D9D9D9" />
      </svg>
      <div
        class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-2 px-3 py-2"
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
            fill-rule="evenodd"
            clip-rule="evenodd"
            d="M11.25 3.75C11.25 2.09315 12.5931 0.75 14.25 0.75C15.9069 0.75 17.25 2.09315 17.25 3.75C17.25 5.40685 15.9069 6.75 14.25 6.75C13.226 6.75 12.3217 6.23691 11.7804 5.45378L6.57602 7.99079C6.68866 8.30617 6.75 8.64592 6.75 9C6.75 9.32963 6.69684 9.64684 6.59862 9.94352L11.7732 12.5567C12.3137 11.7677 13.2214 11.25 14.25 11.25C15.9069 11.25 17.25 12.5931 17.25 14.25C17.25 15.9069 15.9069 17.25 14.25 17.25C12.5931 17.25 11.25 15.9069 11.25 14.25C11.25 14.1587 11.2541 14.0683 11.2621 13.979L5.77885 11.21C5.24477 11.7005 4.53236 12 3.75 12C2.09315 12 0.75 10.6569 0.75 9C0.75 7.34315 2.09315 6 3.75 6C4.50465 6 5.19421 6.27864 5.72143 6.73865L11.2636 4.03701C11.2546 3.94255 11.25 3.84681 11.25 3.75ZM15.75 3.75C15.75 2.92157 15.0784 2.25 14.25 2.25C13.4216 2.25 12.75 2.92157 12.75 3.75C12.75 4.57843 13.4216 5.25 14.25 5.25C15.0784 5.25 15.75 4.57843 15.75 3.75ZM15.75 14.25C15.75 13.4216 15.0784 12.75 14.25 12.75C13.4216 12.75 12.75 13.4216 12.75 14.25C12.75 15.0784 13.4216 15.75 14.25 15.75C15.0784 15.75 15.75 15.0784 15.75 14.25ZM3.75 7.5C4.57843 7.5 5.25 8.17157 5.25 9C5.25 9.82843 4.57843 10.5 3.75 10.5C2.92157 10.5 2.25 9.82843 2.25 9C2.25 8.17157 2.92157 7.5 3.75 7.5Z"
            fill="#232323"
          />
        </svg>
        <p
          class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-[#232323]"
        >
          Share
        </p>
      </div>
      <svg
        width="2"
        height="40"
        viewBox="0 0 2 40"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        class="self-stretch flex-grow-0 flex-shrink-0"
        preserveAspectRatio="none"
      >
        <path d="M1 0V40" stroke="#D9D9D9" />
      </svg>
      <div
        class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-px px-3 py-2"
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
            d="M15.75 4.48511C13.2525 4.23761 10.74 4.11011 8.235 4.11011C6.75 4.11011 5.265 4.18511 3.78 4.33511L2.25 4.48511"
            stroke="#EB5842"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M6.375 3.7275L6.54 2.745C6.66 2.0325 6.75 1.5 8.0175 1.5H9.9825C11.25 1.5 11.3475 2.0625 11.46 2.7525L11.625 3.7275"
            stroke="#EB5842"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M14.1383 6.85498L13.6508 14.4075C13.5683 15.585 13.5008 16.5 11.4083 16.5H6.59328C4.50078 16.5 4.43328 15.585 4.35078 14.4075L3.86328 6.85498"
            stroke="#EB5842"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M7.74805 12.375H10.2455"
            stroke="#EB5842"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M7.125 9.375H10.875"
            stroke="#EB5842"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>
        <p
          class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-[#eb5842]"
        >
          Delete
        </p>
      </div>
    </div>
    <div
      class="flex justify-start items-start w-[360px] absolute left-[51px] top-[66px] gap-6"
    >
      <p
        class="flex-grow w-[312px] text-[32px] font-semibold text-left text-[#232323]"
      >
        Lorem ipsum dolor sit amet consectetur.
      </p>
      <svg
        width="24"
        height="24"
        viewBox="0 0 24 24"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        class="flex-grow-0 flex-shrink-0 w-6 h-6 relative"
        preserveAspectRatio="none"
      >
        <path
          d="M13.2594 3.59997L5.04936 12.29C4.73936 12.62 4.43936 13.27 4.37936 13.72L4.00936 16.96C3.87936 18.13 4.71936 18.93 5.87936 18.73L9.09936 18.18C9.54936 18.1 10.1794 17.77 10.4894 17.43L18.6994 8.73997C20.1194 7.23997 20.7594 5.52997 18.5494 3.43997C16.3494 1.36997 14.6794 2.09997 13.2594 3.59997Z"
          stroke="#9A9A9A"
          stroke-width="1.5"
          stroke-miterlimit="10"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M11.8906 5.05005C12.3206 7.81005 14.5606 9.92005 17.3406 10.2"
          stroke="#9A9A9A"
          stroke-width="1.5"
          stroke-miterlimit="10"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M3 22H21"
          stroke="#9A9A9A"
          stroke-width="1.5"
          stroke-miterlimit="10"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
      </svg>
    </div>
    <div
      class="flex justify-start items-start w-[408px] absolute left-14 top-[195px] gap-4"
    >
      <div
        class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 w-[145px] relative gap-1"
      >
        <p class="flex-grow-0 flex-shrink-0 text-sm text-left text-[#9a9a9a]">
          Visbility
        </p>
        <p
          class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-[#232323]"
        >
          Public
        </p>
      </div>
      <div
        class="flex flex-col justify-start items-start flex-grow relative gap-1"
      >
        <p class="flex-grow-0 flex-shrink-0 text-sm text-left text-[#9a9a9a]">
          License
        </p>
        <p
          class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-[#232323]"
        >
          Non Commercial License
        </p>
      </div>
    </div>
    <div
      class="flex justify-start items-start w-[408px] absolute left-14 top-[268px] gap-4"
    >
      <div
        class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 w-[145px] relative gap-1"
      >
        <p class="flex-grow-0 flex-shrink-0 text-sm text-left text-[#9a9a9a]">
          Created
        </p>
        <p
          class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-[#232323]"
        >
          23 Mar 2022
        </p>
      </div>
      <div
        class="flex flex-col justify-start items-start flex-grow relative gap-1"
      >
        <p class="flex-grow-0 flex-shrink-0 text-sm text-left text-[#9a9a9a]">
          Dimensions
        </p>
        <p
          class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-[#232323]"
        >
          1440 x 1080 pixels
        </p>
      </div>
    </div>
    <div
      class="flex flex-col justify-start items-start absolute left-14 top-[341px] gap-1"
    >
      <p class="flex-grow-0 flex-shrink-0 text-sm text-left text-[#9a9a9a]">
        Model Featured
      </p>
      <p
        class="flex-grow-0 flex-shrink-0 text-base font-medium text-left text-[#232323]"
      >
        Gemma Peach
      </p>
    </div>
    <div
      class="flex flex-col justify-start items-start absolute left-14 top-[419px] gap-1"
    >
      <p class="flex-grow-0 flex-shrink-0 text-sm text-left text-[#9a9a9a]">
        Tags
      </p>
    </div>
    <div class="w-[90px] h-[30px]">
      <div
        class="w-[90px] h-[30px] absolute left-[56.5px] top-[446.5px] bg-[#e0acac]"
      />
      <p
        class="w-[90px] absolute left-[57px] top-[450px] text-base font-medium text-center text-[#232323]"
      >
        Strap Top
      </p>
    </div>
    <div class="w-[90px] h-[30px]">
      <div
        class="w-[90px] h-[30px] absolute left-[150.5px] top-[446.5px] bg-[#ace0be]"
      />
      <p
        class="w-[88px] absolute left-[153px] top-[450px] text-base font-medium text-center text-[#232323]"
      >
        Best
      </p>
    </div>
    <svg
      width="18"
      height="18"
      viewBox="0 0 18 18"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
      class="w-[18px] h-[18px] absolute left-[436px] top-[432px]"
      preserveAspectRatio="none"
    >
      <path
        d="M11.2509 14.9401L6.36086 10.0501C5.78336 9.47256 5.78336 8.52756 6.36086 7.95006L11.2509 3.06006"
        stroke="#1F206C"
        stroke-width="1.5"
        stroke-miterlimit="10"
        stroke-linecap="round"
        stroke-linejoin="round"
      /></svg
    ><svg
      width="18"
      height="18"
      viewBox="0 0 18 18"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
      class="w-[18px] h-[18px] absolute left-[969px] top-[432px]"
      preserveAspectRatio="none"
    >
      <path
        d="M6.68164 14.9401L11.5716 10.0501C12.1491 9.47256 12.1491 8.52756 11.5716 7.95006L6.68164 3.06006"
        stroke="#1F206C"
        stroke-width="1.5"
        stroke-miterlimit="10"
        stroke-linecap="round"
        stroke-linejoin="round"
      />
    </svg>
  </div>
</div>
