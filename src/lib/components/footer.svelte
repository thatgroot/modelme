<script lang="ts">
  import logo from "../../assets/logo.png";
</script>

<div
  class="flex flex-col items-center gap-9 justify-center h-[220px] mt-[103px] px-16 relative overflow-hidden bg-white border-t-[1px] box-border w-[-webkit-fill-available] -ml-14 -mr-14"
  style="border-color:rgba(35, 35, 35, 0.16)"
>
  <div class="flex justify-between items-center w-full">
    <div
      class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-3"
    >
      <img
        src={logo}
        alt="logo"
        class="w-[82.52px] h-[52.12px] object-cover border border-black p-2"
      />
      <p
        class="flex-grow-0 flex-shrink-0 text-[50px] text-left text-neutral-900"
      >
        MODELME
      </p>
    </div>
    <div
      class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-3"
    >
      <span
        class="flex-grow-0 flex-shrink-0 w-[211px] opacity-50 text-lg text-left text-black"
      >
        Sign up to our newsletter
      </span>
      <button
        class="flex justify-start items-center flex-grow-0 flex-shrink-0 relative gap-3 px-8 py-4 bg-white border border-[#1f206c]"
      >
        <span
          class="flex-grow-0 flex-shrink-0 text-lg font-medium text-left text-[#1f206c]"
          >Subscribe</span
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
            d="M14.4297 6.50464L20.4997 12.5746L14.4297 18.6446"
            stroke="#1F206C"
            stroke-width="1.5"
            stroke-miterlimit="10"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M3.5 12.5746H20.33"
            stroke="#1F206C"
            stroke-width="1.5"
            stroke-miterlimit="10"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>
      </button>
    </div>

    <div
      class="flex justify-start items-start flex-grow-0 flex-shrink-0 relative gap-8"
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
          d="M22 16.7646C22 20.4046 19.83 22.5746 16.19 22.5746H15C14.45 22.5746 14 22.1246 14 21.5746V15.8046C14 15.5346 14.22 15.3046 14.49 15.3046L16.25 15.2746C16.39 15.2646 16.51 15.1646 16.54 15.0246L16.89 13.1146C16.92 12.9346 16.78 12.7646 16.59 12.7646L14.46 12.7946C14.18 12.7946 13.96 12.5746 13.95 12.3046L13.91 9.85458C13.91 9.69458 14.04 9.5546 14.21 9.5546L16.61 9.51459C16.78 9.51459 16.91 9.3846 16.91 9.2146L16.87 6.81458C16.87 6.64458 16.74 6.51459 16.57 6.51459L13.87 6.5546C12.21 6.5846 10.89 7.94458 10.92 9.60458L10.97 12.3546C10.98 12.6346 10.76 12.8546 10.48 12.8646L9.28 12.8846C9.11 12.8846 8.98001 13.0146 8.98001 13.1846L9.01001 15.0846C9.01001 15.2546 9.14 15.3846 9.31 15.3846L10.51 15.3646C10.79 15.3646 11.01 15.5846 11.02 15.8546L11.11 21.5546C11.12 22.1146 10.67 22.5746 10.11 22.5746H7.81C4.17 22.5746 2 20.4046 2 16.7546V8.38458C2 4.74458 4.17 2.57458 7.81 2.57458H16.19C19.83 2.57458 22 4.74458 22 8.38458V16.7646V16.7646Z"
          fill="#1F206C"
        />
      </svg>
      <svg
        width="24"
        height="25"
        viewBox="0 0 24 25"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        class="flex-grow-0 flex-shrink-0 w-6 h-6 relative"
        preserveAspectRatio="xMidYMid meet"
      >
        <path
          d="M7.54752 22.3252C16.6042 22.3252 21.5578 14.8219 21.5578 8.31498C21.5578 8.10186 21.5578 7.8897 21.5434 7.6785C22.507 6.98146 23.3389 6.11839 24 5.1297C23.1014 5.5281 22.148 5.78926 21.1718 5.90442C22.1998 5.28911 22.9692 4.32121 23.3366 3.1809C22.3701 3.75451 21.3126 4.15873 20.2099 4.3761C19.4675 3.58668 18.4856 3.06394 17.4162 2.88879C16.3468 2.71363 15.2494 2.89582 14.294 3.40716C13.3385 3.91849 12.5782 4.73048 12.1307 5.71745C11.6833 6.70443 11.5735 7.81137 11.8186 8.86698C9.86089 8.76878 7.94576 8.26001 6.19745 7.37371C4.44915 6.4874 2.90676 5.24336 1.6704 3.72234C1.04073 4.80634 0.847872 6.08957 1.1311 7.31077C1.41433 8.53196 2.15234 9.5993 3.19488 10.2955C2.41123 10.2725 1.64465 10.0611 0.96 9.67914V9.74154C0.960311 10.8784 1.35385 11.9801 2.07387 12.8599C2.79389 13.7397 3.79606 14.3433 4.9104 14.5684C4.18548 14.7662 3.42487 14.7951 2.68704 14.6529C3.00181 15.6312 3.61443 16.4867 4.43924 17.0998C5.26405 17.7129 6.25983 18.053 7.28736 18.0724C6.26644 18.8749 5.09731 19.4682 3.84687 19.8184C2.59643 20.1686 1.28921 20.2689 0 20.1134C2.25183 21.5584 4.87192 22.3249 7.54752 22.3214"
          fill="#1F206C"
        />
      </svg>
      <svg
        width="24"
        height="25"
        viewBox="0 0 24 25"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        class="flex-grow-0 flex-shrink-0 w-6 h-6 relative"
        preserveAspectRatio="xMidYMid meet"
      >
        <g clip-path="url(#clip0_25_6148)">
          <path
            d="M20.317 4.93438C18.7873 4.23251 17.147 3.71539 15.4319 3.41921C15.4007 3.4135 15.3694 3.42778 15.3534 3.45635C15.1424 3.83157 14.9087 4.32108 14.7451 4.70582C12.9004 4.42964 11.0652 4.42964 9.25831 4.70582C9.09466 4.3125 8.85248 3.83157 8.64058 3.45635C8.6245 3.42873 8.59328 3.41445 8.56206 3.41921C6.84792 3.71444 5.20756 4.23156 3.67694 4.93438C3.66369 4.9401 3.65234 4.94962 3.64477 4.962C0.533392 9.61037 -0.31895 14.1445 0.0991801 18.6224C0.101072 18.6443 0.11337 18.6652 0.130398 18.6785C2.18321 20.1861 4.17169 21.1013 6.12328 21.7079C6.1545 21.7175 6.18761 21.706 6.20748 21.6803C6.66912 21.0499 7.08063 20.3851 7.43349 19.6861C7.4543 19.6452 7.43443 19.5966 7.39186 19.5804C6.73913 19.3328 6.11761 19.0309 5.51974 18.6881C5.47244 18.6604 5.46865 18.5928 5.51217 18.5604C5.63799 18.4662 5.76381 18.3681 5.88395 18.269C5.9057 18.2509 5.93598 18.2471 5.96152 18.2586C9.88929 20.0518 14.1415 20.0518 18.023 18.2586C18.0485 18.2462 18.0788 18.25 18.1015 18.2681C18.2216 18.3671 18.3474 18.4662 18.4742 18.5604C18.5177 18.5928 18.5149 18.6604 18.4676 18.6881C17.8697 19.0376 17.2482 19.3328 16.5945 19.5795C16.5519 19.5956 16.533 19.6452 16.5538 19.6861C16.9143 20.3842 17.3258 21.0489 17.7789 21.6794C17.7978 21.706 17.8319 21.7175 17.8631 21.7079C19.8241 21.1013 21.8126 20.1861 23.8654 18.6785C23.8834 18.6652 23.8948 18.6452 23.8967 18.6233C24.3971 13.4464 23.0585 8.94944 20.3482 4.96295C20.3416 4.94962 20.3303 4.9401 20.317 4.93438ZM8.02001 15.8958C6.83751 15.8958 5.86313 14.8101 5.86313 13.4769C5.86313 12.1436 6.81859 11.0579 8.02001 11.0579C9.23088 11.0579 10.1958 12.1531 10.1769 13.4769C10.1769 14.8101 9.22142 15.8958 8.02001 15.8958ZM15.9948 15.8958C14.8123 15.8958 13.8379 14.8101 13.8379 13.4769C13.8379 12.1436 14.7933 11.0579 15.9948 11.0579C17.2056 11.0579 18.1705 12.1531 18.1516 13.4769C18.1516 14.8101 17.2056 15.8958 15.9948 15.8958Z"
            fill="#1F206C"
          />
        </g>
        <defs>
          <clipPath id="clip0_25_6148">
            <rect
              width="24"
              height="24"
              fill="white"
              transform="translate(0 0.574585)"
            />
          </clipPath>
        </defs>
      </svg>
      <svg
        width="24"
        height="25"
        viewBox="0 0 24 25"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        class="flex-grow-0 flex-shrink-0 w-6 h-6 relative"
        preserveAspectRatio="xMidYMid meet"
      >
        <path
          d="M3.5 5.28125C3.5 4.61483 4.04024 4.07458 4.70666 4.07458H19.2933C19.9598 4.07458 20.5 4.61483 20.5 5.28125V19.8679C20.5 20.5343 19.9598 21.0745 19.2933 21.0745H4.70667C4.04024 21.0745 3.5 20.5343 3.5 19.8679V5.28125Z"
          fill="#1F206C"
        />
        <path
          d="M7.31654 9.35403C8.13102 9.35403 8.79129 8.69377 8.79129 7.87929C8.79129 7.06481 8.13102 6.40454 7.31654 6.40454C6.50206 6.40454 5.8418 7.06481 5.8418 7.87929C5.8418 8.69377 6.50206 9.35403 7.31654 9.35403Z"
          fill="white"
        />
        <path
          d="M10.1419 10.4439H12.586V11.5636C12.586 11.5636 13.2493 10.2371 15.0539 10.2371C16.6637 10.2371 17.9972 11.0301 17.9972 13.4473V18.5444H15.4644V14.0649C15.4644 12.639 14.7031 12.4822 14.123 12.4822C12.9192 12.4822 12.7131 13.5206 12.7131 14.2509V18.5444H10.1419V10.4439Z"
          fill="white"
        />
        <path
          d="M6.03097 10.4439H8.60212V18.5444H6.03097V10.4439Z"
          fill="white"
        />
      </svg>
    </div>
  </div>

  <div class="flex justify-between items-center w-full">
    <span
      class="flex-grow-0 flex-shrink-0 opacity-50 text-lg text-left text-black"
    >
      © 2023 ModelMe UG (haftungsbeschränkt), All rights reserved.
    </span>
    <div
      class="flex justify-start items-start flex-grow-0 flex-shrink-0 relative opacity-50 gap-12"
    >
      <span class="flex-grow-0 flex-shrink-0 text-lg text-left text-black">
        Privacy Policy
      </span>
      <span class="flex-grow-0 flex-shrink-0 text-lg text-left text-black">
        Terms &#x26; Conditions
      </span>
      <span class="flex-grow-0 flex-shrink-0 text-lg text-left text-black">
        Cookies
      </span>
    </div>
  </div>
</div>
