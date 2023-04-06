<script>
  import Input from "../../input.svelte";
</script>

<div class="flex flex-col justify-start items-start max-w-3xl gap-6">
  <div
    class="flex flex-col justify-start items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-8"
  >
    <p
      class="flex-grow-0 flex-shrink-0 text-lg font-semibold text-left text-[#232323]"
    >
      Manage Team Members
    </p>
    <div
      class="flex justify-start items-end self-stretch flex-grow-0 flex-shrink-0 gap-4"
    >
      <div
        class="flex flex-col justify-start items-start flex-grow relative gap-2"
      >
        <p
          class="flex-grow-0 flex-shrink-0 w-[327px] text-sm font-semibold text-left text-[#232323]"
        >
          Email
        </p>

        <Input
          name="email"
          type="email"
          placeholder="ganteng@mail.com"
          width="w-full"
        />
      </div>
      <div
        class="flex justify-center items-center flex-grow-0 flex-shrink-0 w-36 relative gap-2 p-4 bg-[#1f206c]"
      >
        <p
          class="flex-grow-0 flex-shrink-0 text-base font-medium text-center text-white"
        >
          Invite
        </p>
      </div>
    </div>
  </div>
  <div
    class="flex flex-col justify-start items-start self-stretch flex-grow-0 flex-shrink-0 gap-4"
  >
    <div
      class="flex justify-start items-center self-stretch flex-grow-0 flex-shrink-0 gap-8"
    >
      <div class="flex justify-start items-center flex-grow relative gap-4">
        <img class="flex-grow-0 flex-shrink-0" src="ellipse-428.png" />
        <div
          class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 relative"
        >
          <p
            class="flex-grow-0 flex-shrink-0 text-xs font-medium text-left text-[#232323]"
          >
            Ganteng
          </p>
          <p class="flex-grow-0 flex-shrink-0 text-xs text-left text-[#9a9a9a]">
            ganteng@mail.com
          </p>
        </div>
      </div>
      <div
        class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-2"
      >
        <p
          class="flex-grow-0 flex-shrink-0 text-xs font-medium text-left text-[#9a9a9a]"
        >
          Can view
        </p>
        <svg
          width="12"
          height="12"
          viewBox="0 0 12 12"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          class="flex-grow-0 flex-shrink-0 w-3 h-3 relative"
          preserveAspectRatio="xMidYMid meet"
        >
          <path
            d="M9.95906 4.4751L6.69906 7.7351C6.31406 8.1201 5.68406 8.1201 5.29906 7.7351L2.03906 4.4751"
            stroke="#9A9A9A"
            stroke-width="1.5"
            stroke-miterlimit="10"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>
      </div>
      <div
        class="flex justify-start items-start flex-grow-0 flex-shrink-0 relative gap-2"
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
          class="flex-grow-0 flex-shrink-0 text-xs font-medium text-left text-[#eb5842]"
        >
          Delete
        </p>
      </div>
    </div>
    <div
      class="flex justify-start items-center self-stretch flex-grow-0 flex-shrink-0 gap-8"
    >
      <div class="flex justify-start items-center flex-grow relative gap-4">
        <img class="flex-grow-0 flex-shrink-0" src="ellipse-428.png" />
        <div
          class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 relative"
        >
          <p
            class="flex-grow-0 flex-shrink-0 text-xs font-medium text-left text-[#232323]"
          >
            Ganteng
          </p>
          <p class="flex-grow-0 flex-shrink-0 text-xs text-left text-[#9a9a9a]">
            ganteng@mail.com
          </p>
        </div>
      </div>
      <div
        class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-2"
      >
        <p
          class="flex-grow-0 flex-shrink-0 text-xs font-medium text-left text-[#9a9a9a]"
        >
          Can edit
        </p>
        <svg
          width="12"
          height="12"
          viewBox="0 0 12 12"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          class="flex-grow-0 flex-shrink-0 w-3 h-3 relative"
          preserveAspectRatio="xMidYMid meet"
        >
          <path
            d="M9.95906 4.4751L6.69906 7.7351C6.31406 8.1201 5.68406 8.1201 5.29906 7.7351L2.03906 4.4751"
            stroke="#9A9A9A"
            stroke-width="1.5"
            stroke-miterlimit="10"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>
      </div>
      <div
        class="flex justify-start items-start flex-grow-0 flex-shrink-0 relative gap-2"
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
          class="flex-grow-0 flex-shrink-0 text-xs font-medium text-left text-[#eb5842]"
        >
          Delete
        </p>
      </div>
    </div>
    <div
      class="flex justify-start items-center self-stretch flex-grow-0 flex-shrink-0 gap-8"
    >
      <div class="flex justify-start items-center flex-grow relative gap-4">
        <img class="flex-grow-0 flex-shrink-0" src="ellipse-428.png" />
        <div
          class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 relative"
        >
          <p
            class="flex-grow-0 flex-shrink-0 text-xs font-medium text-left text-[#232323]"
          >
            Ganteng
          </p>
          <p class="flex-grow-0 flex-shrink-0 text-xs text-left text-[#9a9a9a]">
            ganteng@mail.com
          </p>
        </div>
      </div>
      <div
        class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-2"
      >
        <p
          class="flex-grow-0 flex-shrink-0 text-xs font-medium text-left text-[#9a9a9a]"
        >
          Can edit
        </p>
        <svg
          width="12"
          height="12"
          viewBox="0 0 12 12"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          class="flex-grow-0 flex-shrink-0 w-3 h-3 relative"
          preserveAspectRatio="xMidYMid meet"
        >
          <path
            d="M9.95906 4.4751L6.69906 7.7351C6.31406 8.1201 5.68406 8.1201 5.29906 7.7351L2.03906 4.4751"
            stroke="#9A9A9A"
            stroke-width="1.5"
            stroke-miterlimit="10"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>
      </div>
      <div
        class="flex justify-start items-start flex-grow-0 flex-shrink-0 relative gap-2"
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
          class="flex-grow-0 flex-shrink-0 text-xs font-medium text-left text-[#eb5842]"
        >
          Delete
        </p>
      </div>
    </div>
  </div>
  <div
    class="flex justify-center items-center self-stretch flex-grow-0 flex-shrink-0 relative gap-2 p-3 bg-[#e9e9e9]"
  >
    <p
      class="flex-grow-0 flex-shrink-0 text-sm font-medium text-center text-[#232323]"
    >
      Show All Team Members
    </p>
  </div>
</div>

<style>
  p {
    font-family: var(--theme-font-family-base);
  }
</style>
