<script lang="ts">
  import login_image from "../../assets/login.png";
  import CheckboxBlue from "./checkbox-blue.svelte";
  import Checkbox from "./checkbox.svelte";
  import Input from "./input.svelte";
</script>

<div
  class="flex justify-center items-start flex-grow-0 flex-shrink-0 relative bg-white"
>
  <img
    class="self-stretch flex-grow-0 flex-shrink-0 w-[550px]"
    src={login_image}
    alt="..."
  />
  <div
    class="flex flex-col justify-start items-center flex-grow-0 flex-shrink-0 gap-4 px-8 pt-8 pb-[72px]"
  >
    <div
      class="flex justify-end items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-2.5"
    >
      <svg
        width="25"
        height="25"
        viewBox="0 0 25 25"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        class="flex-grow-0 flex-shrink-0 w-6 h-6 relative"
        preserveAspectRatio="none"
      >
        <path
          d="M5.5 5.5L19.4991 19.4991"
          stroke="#232323"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M5.50094 19.4991L19.5 5.5"
          stroke="#232323"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
      </svg>
    </div>
    <div
      class="flex flex-col justify-start items-center flex-grow-0 flex-shrink-0 relative gap-6 p-6 bg-white"
    >
      <div
        class="flex flex-col justify-center items-center flex-grow-0 flex-shrink-0 relative gap-2"
      >
        <span
          class="flex-grow-0 flex-shrink-0 w-[327px] text-2xl font-bold text-center text-[#232323]"
        >
          Welcome back!
        </span>
      </div>
      <div
        class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 relative gap-2"
      >
        <span
          class="flex-grow-0 flex-shrink-0 w-[327px] text-sm font-semibold text-left text-[#232323]"
        >
          Email
        </span>
        <Input
          name="email"
          type="email"
          placeholder="ganteng@mail.com"
          width="w-full"
        />
      </div>
      <div
        class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 relative gap-2"
      >
        <span
          class="flex-grow-0 flex-shrink-0 w-[327px] text-sm font-semibold text-left text-[#232323]"
        >
          Password
        </span>
        <Input
          name="password"
          type="password"
          placeholder="********"
          width="w-full"
        />
      </div>
      <div
        class="flex justify-between items-center flex-grow-0 flex-shrink-0 w-[327px] relative"
      >
        <div
          class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-3"
        >
          <CheckboxBlue name="remember" />
          <span
            class="flex-grow-0 flex-shrink-0 text-sm font-medium text-left text-[#232323]"
          >
            Remember me
          </span>
        </div>
        <a
          href="#!"
          class="flex-grow-0 flex-shrink-0 text-sm font-medium text-left text-[#1f206c]"
        >
          Forgot passwrod?
        </a>
      </div>
      <button
        class="flex justify-center items-center flex-grow-0 flex-shrink-0 w-[327px] relative gap-2 p-4 bg-[#1f206c]"
      >
        <span
          class="flex-grow-0 flex-shrink-0 text-base font-medium text-center text-white"
        >
          Login
        </span>
      </button>
      <div
        class="flex justify-center items-center flex-grow-0 flex-shrink-0 w-[327px] relative gap-3"
      >
        <svg
          width="144"
          height="2"
          viewBox="0 0 144 2"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          class="flex-grow"
          preserveAspectRatio="none"
        >
          <path d="M0.5 1H144" stroke="#D9D9D9" />
        </svg>
        <span
          class="flex-grow-0 flex-shrink-0 text-sm font-medium text-left text-[#9a9a9a]"
          >Or</span
        >
        <svg
          width="144"
          height="2"
          viewBox="0 0 144 2"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          class="flex-grow"
          preserveAspectRatio="none"
        >
          <path d="M0 1H143.5" stroke="#D9D9D9" />
        </svg>
      </div>
      <div
        class="flex justify-center items-center flex-grow-0 flex-shrink-0 w-[327px] gap-3.5"
      >
        <div
          class="flex justify-center items-center flex-grow relative gap-2 p-3 border border-[#1f206c]"
        >
          <svg
            width="19"
            height="19"
            viewBox="0 0 19 19"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            class="flex-grow-0 flex-shrink-0 w-[18px] h-[18px] relative"
            preserveAspectRatio="xMidYMid meet"
          >
            <g clip-path="url(#clip0_164_4341)">
              <path
                d="M18.5914 9.66863C18.5914 8.93117 18.5302 8.39303 18.3976 7.83496H9.7793V11.1634H14.8381C14.7361 11.9906 14.1854 13.2363 12.9614 14.0734L12.9443 14.1848L15.6692 16.2475L15.858 16.2659C17.5919 14.7013 18.5914 12.3992 18.5914 9.66863Z"
                fill="#1F206C"
              />
              <path
                d="M9.77832 18.4384C12.2567 18.4384 14.3373 17.6411 15.857 16.2659L12.9605 14.0734C12.1853 14.6015 11.145 14.9703 9.77832 14.9703C7.35092 14.9703 5.29069 13.4057 4.55628 11.2432L4.44863 11.2521L1.61518 13.3947L1.57812 13.4954C3.08759 16.4252 6.18816 18.4384 9.77832 18.4384Z"
                fill="#1F206C"
              />
              <path
                d="M4.55687 11.2431C4.36309 10.685 4.25094 10.087 4.25094 9.4692C4.25094 8.85129 4.36309 8.25338 4.54667 7.69531L4.54154 7.57645L1.67258 5.39941L1.57871 5.44304C0.956586 6.65887 0.599609 8.02419 0.599609 9.4692C0.599609 10.9142 0.956586 12.2795 1.57871 13.4953L4.55687 11.2431Z"
                fill="#1F206C"
              />
              <path
                d="M9.77832 3.96802C11.502 3.96802 12.6646 4.69551 13.3276 5.30346L15.9182 2.83196C14.3272 1.38695 12.2567 0.5 9.77832 0.5C6.18816 0.5 3.08759 2.51305 1.57812 5.44292L4.54609 7.69519C5.2907 5.53265 7.35092 3.96802 9.77832 3.96802Z"
                fill="#1F206C"
              />
            </g>
            <defs>
              <clipPath id="clip0_164_4341">
                <rect
                  width="18"
                  height="18"
                  fill="white"
                  transform="translate(0.599609 0.5)"
                />
              </clipPath>
            </defs>
          </svg>
        </div>
        <div
          class="flex justify-center items-center flex-grow relative gap-2 p-3 border border-[#1f206c]"
        >
          <svg
            width="19"
            height="19"
            viewBox="0 0 19 19"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            class="flex-grow-0 flex-shrink-0 w-[18px] h-[18px] relative"
            preserveAspectRatio="xMidYMid meet"
          >
            <path
              d="M8.67383 16.175C5.48633 15.6125 3.04883 12.8375 3.04883 9.5C3.04883 5.7875 6.08633 2.75 9.79883 2.75C13.5113 2.75 16.5488 5.7875 16.5488 9.5C16.5488 12.8375 14.1113 15.6125 10.9238 16.175L10.5488 15.875H9.04883L8.67383 16.175Z"
              fill="#1F206C"
            />
            <path
              d="M12.4238 11.375L12.7238 9.5H10.9238V8.1875C10.9238 7.6625 11.1113 7.25 11.9363 7.25H12.7988V5.525C12.3113 5.45 11.7863 5.375 11.2988 5.375C9.76133 5.375 8.67383 6.3125 8.67383 8V9.5H6.98633V11.375H8.67383V16.1375C9.04883 16.2125 9.42383 16.25 9.79883 16.25C10.1738 16.25 10.5488 16.2125 10.9238 16.1375V11.375H12.4238Z"
              fill="white"
            />
          </svg>
        </div>
        <div
          class="flex justify-center items-center flex-grow relative gap-2 p-3 border border-[#1f206c]"
        >
          <svg
            width="18"
            height="19"
            viewBox="0 0 18 19"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            class="flex-grow-0 flex-shrink-0 w-[18px] h-[18px] relative"
            preserveAspectRatio="xMidYMid meet"
          >
            <path
              d="M2.625 4.03C2.625 3.53018 3.03018 3.125 3.53 3.125H14.47C14.9698 3.125 15.375 3.53018 15.375 4.03V14.97C15.375 15.4698 14.9698 15.875 14.47 15.875H3.53C3.03018 15.875 2.625 15.4698 2.625 14.97V4.03Z"
              fill="#1F206C"
            />
            <path
              d="M5.48692 7.08468C6.09778 7.08468 6.59298 6.58948 6.59298 5.97862C6.59298 5.36776 6.09778 4.87256 5.48692 4.87256C4.87606 4.87256 4.38086 5.36776 4.38086 5.97862C4.38086 6.58948 4.87606 7.08468 5.48692 7.08468Z"
              fill="white"
            />
            <path
              d="M7.60594 7.90209H9.43904V8.74184C9.43904 8.74184 9.93647 7.74697 11.2899 7.74697C12.4973 7.74697 13.4974 8.34173 13.4974 10.1546V13.9775H11.5978V10.6178C11.5978 9.54841 11.0269 9.43079 10.5918 9.43079C9.68888 9.43079 9.5343 10.2096 9.5343 10.7573V13.9775H7.60594V7.90209Z"
              fill="white"
            />
            <path
              d="M4.52274 7.90209H6.4511V13.9775H4.52274V7.90209Z"
              fill="white"
            />
          </svg>
        </div>
        <div
          class="flex justify-center items-center flex-grow relative gap-2 p-3 border border-[#1f206c]"
        >
          <svg
            width="19"
            height="19"
            viewBox="0 0 19 19"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            class="flex-grow-0 flex-shrink-0 w-[18px] h-[18px] relative"
            preserveAspectRatio="xMidYMid meet"
          >
            <g clip-path="url(#clip0_164_2958)">
              <path
                d="M15.437 3.76963C14.2897 3.24323 13.0595 2.85539 11.7731 2.63326C11.7497 2.62897 11.7263 2.63968 11.7142 2.66111C11.556 2.94253 11.3808 3.30965 11.258 3.59821C9.87452 3.39108 8.49809 3.39108 7.14295 3.59821C7.02021 3.30323 6.83858 2.94253 6.67965 2.66111C6.66759 2.6404 6.64418 2.62968 6.62076 2.63326C5.33516 2.85467 4.10489 3.24251 2.95692 3.76963C2.94699 3.77392 2.93847 3.78106 2.9328 3.79035C0.599263 7.27662 -0.0399939 10.6772 0.273604 14.0356C0.275023 14.052 0.284246 14.0678 0.297017 14.0778C1.83663 15.2084 3.32799 15.8948 4.79168 16.3498C4.81509 16.3569 4.83993 16.3484 4.85483 16.3291C5.20106 15.8562 5.50969 15.3577 5.77433 14.8334C5.78994 14.8027 5.77504 14.7663 5.74312 14.7542C5.25356 14.5684 4.78742 14.342 4.33902 14.0849C4.30355 14.0642 4.30071 14.0135 4.33335 13.9892C4.42771 13.9185 4.52207 13.8449 4.61218 13.7706C4.6285 13.7571 4.6512 13.7542 4.67036 13.7628C7.61619 15.1077 10.8054 15.1077 13.7164 13.7628C13.7356 13.7535 13.7583 13.7563 13.7753 13.7699C13.8654 13.8442 13.9598 13.9185 14.0549 13.9892C14.0875 14.0135 14.0854 14.0642 14.0499 14.0849C13.6015 14.347 13.1354 14.5684 12.6451 14.7534C12.6132 14.7656 12.599 14.8027 12.6146 14.8334C12.8849 15.357 13.1935 15.8555 13.5334 16.3284C13.5476 16.3484 13.5731 16.3569 13.5965 16.3498C15.0673 15.8948 16.5587 15.2084 18.0983 14.0778C18.1118 14.0678 18.1203 14.0528 18.1217 14.0363C18.497 10.1536 17.4931 6.78093 15.4604 3.79106C15.4554 3.78106 15.4469 3.77392 15.437 3.76963ZM6.21422 11.9907C5.32735 11.9907 4.59657 11.1765 4.59657 10.1765C4.59657 9.17654 5.31316 8.36229 6.21422 8.36229C7.12238 8.36229 7.84607 9.18368 7.83188 10.1765C7.83188 11.1765 7.11528 11.9907 6.21422 11.9907ZM12.1953 11.9907C11.3084 11.9907 10.5776 11.1765 10.5776 10.1765C10.5776 9.17654 11.2942 8.36229 12.1953 8.36229C13.1034 8.36229 13.8271 9.18368 13.8129 10.1765C13.8129 11.1765 13.1034 11.9907 12.1953 11.9907Z"
                fill="#1F206C"
              />
            </g>
            <defs>
              <clipPath id="clip0_164_2958">
                <rect
                  width="18"
                  height="18"
                  fill="white"
                  transform="translate(0.199219 0.5)"
                />
              </clipPath>
            </defs>
          </svg>
        </div>
        <div
          class="flex justify-center items-center flex-grow relative gap-2 p-3 border border-[#1f206c]"
        >
          <svg
            width="19"
            height="19"
            viewBox="0 0 19 19"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            class="flex-grow-0 flex-shrink-0 w-[18px] h-[18px] relative"
            preserveAspectRatio="xMidYMid meet"
          >
            <path
              fill-rule="evenodd"
              clip-rule="evenodd"
              d="M15.2283 6.56672C15.2333 6.69788 15.235 6.82899 15.235 6.96016C15.235 10.9368 12.4377 15.5276 7.32221 15.5276C5.75084 15.5276 4.28969 15.0268 3.05859 14.1742C3.27621 14.1981 3.49722 14.216 3.72163 14.216C5.02451 14.216 6.22452 13.733 7.17638 12.9222C5.95942 12.9043 4.93181 12.0279 4.57741 10.8355C4.74754 10.8712 4.92276 10.8892 5.10194 10.8892C5.3546 10.8892 5.59991 10.8534 5.83506 10.7819C4.56157 10.5076 3.60236 9.29142 3.60236 7.83073C3.60236 7.81285 3.60236 7.80685 3.60236 7.79492C3.97768 8.01552 4.40726 8.15257 4.86341 8.17046C4.11616 7.62792 3.62496 6.70383 3.62496 5.66048C3.62496 5.11198 3.76175 4.59326 4.00254 4.14611C5.37382 5.97048 7.42396 7.16886 9.73524 7.29406C9.68776 7.07347 9.66345 6.84101 9.66345 6.60849C9.66345 4.9451 10.9087 3.59766 12.445 3.59766C13.2448 3.59766 13.9672 3.96139 14.4742 4.54567C15.109 4.4145 15.7036 4.16412 16.2417 3.81832C16.0332 4.52184 15.5928 5.11195 15.0174 5.48159C15.5804 5.41005 16.1174 5.2492 16.6154 5.01072C16.2417 5.61288 15.7715 6.14342 15.2283 6.56672Z"
              fill="#1F206C"
            />
          </svg>
        </div>
      </div>
      <span class="flex items-center gap-1 text-sm font-medium text-left">
        <span class=" text-sm font-medium text-left text-[#9a9a9a]">
          Don’t have an account?
        </span>
        <span class=" text-sm font-medium text-left text-[#1f206c]">
          Register
        </span>
      </span>
    </div>
  </div>
</div>
