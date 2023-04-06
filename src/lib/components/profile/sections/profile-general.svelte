<script lang="ts">
  import image_19 from "../../../../assets/19.png";
  import image_37 from "../../../../assets/37.png";
  import image_38 from "../../../../assets/38.png";
  import image_39 from "../../../../assets/39.png";
  import Badge from "../../badge.svelte";
  import Input from "../../input.svelte";
  import SubscriptionOverlay from "../../subscription-overlay.svelte";

  export let subscriptions: Array<{
    title: string;
    pricing: {
      period: "mo" | "yr";
      currency: string | "€" | "$";
      amount: number;
    }[];
    subtitle: string;
    perks: Array<string>;
  }> = [];
</script>

<div
  class="flex flex-col justify-start items-start w-[1333px] relative gap-8 p-8 bg-white"
>
  <div
    class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 w-[600px] relative gap-4"
  >
    <p
      class="flex-grow-0 flex-shrink-0 text-lg font-semibold text-left text-[#232323]"
    >
      Account Information
    </p>
    <div
      class="flex flex-col justify-start items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-2"
    >
      <p
        class="flex-grow-0 flex-shrink-0 w-[327px] text-sm font-semibold text-left text-[#232323]"
      >
        Email
      </p>
      <Input
        placeholder="ganteng@mail.com"
        type="email"
        name="email"
        id="email"
        width="w-full"
      />
    </div>
    <div
      class="flex flex-col justify-start items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-2"
    >
      <p
        class="flex-grow-0 flex-shrink-0 w-[327px] text-sm font-semibold text-left text-[#232323]"
      >
        Password
      </p>
      <Input
        type="password"
        placeholder="********"
        name="password"
        id="password"
        width="w-full"
      />
    </div>
  </div>
  <div
    class="flex flex-col justify-start items-start self-stretch flex-grow-0 flex-shrink-0 relative gap-4"
  >
    <p
      class="flex-grow-0 flex-shrink-0 text-lg font-semibold text-left text-[#232323]"
    >
      Subscriptions
    </p>
    <!-- {#each subscriptions as { title, subtitle, pricing, perks }} -->
    <div class="flex justify-center items-center h-[600px] gap-6">
      <div
        class="group flex flex-col justify-start items-center self-stretch w-[408px] p-10 relative overflow-hidden gap-[25px] bg-[#e3e4dd]"
      >
        <div
          class="flex flex-col justify-start items-start relative opacity-0"
        >
          <span
            class="text-[32px] font-semibold text-left text-neutral-900 leading-[39px]"
          >
            High Grade (HG)
          </span>
          <span class="text-[32px] font-semibold text-left text-neutral-900">
            €30/mo | €288/yr
          </span>
        </div>
        <img
          src={image_38}
          alt="..."
          class="absolute -bottom-10 pt-4 z-0 object-cover blur-3xl"
        />
        <SubscriptionOverlay active={true}>
          <div class="absolute -bottom-7 -right-8">
            <Badge lable="Most popular" />
          </div>
        </SubscriptionOverlay>
      </div>
      <div
        class="group flex flex-col justify-start items-center self-stretch w-[408px] p-10 relative overflow-hidden gap-[25px] bg-[#e3e4dd]"
      >
        <div
          class="flex flex-col justify-start items-start relative opacity-0"
        >
          <span
            class="text-[32px] font-semibold text-left text-neutral-900 leading-[39px]"
          >
            Real Grade (RG)
          </span>
          <span class="text-[32px] font-semibold text-left text-neutral-900">
            €60/mo | €576/yr
          </span>
        </div>
        <img
          src={image_39}
          alt="..."
          class="absolute -bottom-10 pt-4 z-0 object-cover blur-3xl"
        />
        <SubscriptionOverlay active={true}>
          <div class="absolute -bottom-7 -right-8">
            <Badge lable="Best value" />
          </div>
        </SubscriptionOverlay>
      </div>
      <div
        class="group flex flex-col justify-start items-center self-stretch w-[408px] p-10 relative overflow-hidden gap-[25px] bg-[#e3e4dd]"
      >
        <div
          class="flex flex-col justify-start items-start relative opacity-0"
        >
          <span
            class="text-[32px] font-semibold text-left text-neutral-900 leading-[39px]"
          >
            Entry Grade (EG)
          </span>
          <span class="text-[32px] font-semibold text-left text-neutral-900">
            €10/mo | €96/yr
          </span>
        </div>
        <img
          src={image_37}
          alt="..."
          class="absolute -bottom-10 pt-4 z-0 object-cover blur-3xl"
        />
        <SubscriptionOverlay active={true} />
      </div>
    </div>
    <!-- {/each} -->
  </div>
  <div
    class="flex flex-col justify-start items-start flex-grow-0 flex-shrink-0 w-[347px] relative gap-4"
  >
    <p
      class="flex-grow-0 flex-shrink-0 text-lg font-semibold text-left text-[#232323]"
    >
      Payment
    </p>
    <div
      class="flex justify-start items-center self-stretch flex-grow-0 flex-shrink-0 relative gap-4"
    >
      <svg
        width="64"
        height="32"
        viewBox="0 0 64 32"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        class="flex-grow-0 flex-shrink-0 w-16 h-8 relative"
        preserveAspectRatio="xMidYMid meet"
      >
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M27.3943 27.1864L27.8305 24.5446L26.8588 24.523H22.2188L25.4434 5.02764C25.4535 4.96861 25.4859 4.91381 25.5334 4.87482C25.581 4.83584 25.6418 4.81445 25.7053 4.81445H33.5291C36.1267 4.81445 37.9192 5.32972 38.8549 6.34689C39.2937 6.82407 39.5731 7.32285 39.7084 7.87154C39.8502 8.4474 39.8525 9.13532 39.7142 9.97449L39.7042 10.0355V10.5733L40.1429 10.8103C40.5123 10.9972 40.806 11.2111 41.0312 11.4559C41.4064 11.864 41.6492 12.3826 41.7518 12.9973C41.8578 13.6295 41.8228 14.382 41.6492 15.2339C41.449 16.2136 41.1254 17.0671 40.6882 17.7652C40.2864 18.4086 39.7743 18.9424 39.1661 19.3558C38.5855 19.7488 37.8958 20.0471 37.1159 20.238C36.3601 20.4256 35.4985 20.5202 34.5534 20.5202H33.9445C33.5093 20.5202 33.0864 20.6697 32.7544 20.9377C32.4215 21.2113 32.2014 21.5851 32.1339 21.9939L32.0878 22.2318L31.3171 26.8884L31.2822 27.0592C31.2729 27.1134 31.257 27.1403 31.2336 27.1586C31.2129 27.1753 31.1829 27.1864 31.1537 27.1864H27.3943"
          fill="#28356A"
        />
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M40.5587 10.0977C40.5356 10.24 40.5087 10.3855 40.4788 10.535C39.4471 15.5861 35.917 17.331 31.4088 17.331H29.1133C28.5619 17.331 28.0972 17.7126 28.0114 18.2312L26.5033 27.3526C26.4475 27.6932 26.7227 28 27.083 28H31.1543C31.6363 28 32.0459 27.666 32.1218 27.2127L32.1618 27.0155L32.9283 22.3772L32.9776 22.1228C33.0526 21.6679 33.4631 21.3338 33.9451 21.3338H34.554C38.4985 21.3338 41.5865 19.8069 42.489 15.388C42.8659 13.5421 42.6708 12.0008 41.6732 10.9168C41.3713 10.59 40.9968 10.3186 40.5587 10.0977"
          fill="#019DDE"
        />
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M39.4798 9.68708C39.3221 9.64319 39.1595 9.60354 38.9927 9.56767C38.8249 9.5327 38.6532 9.50173 38.4763 9.47455C37.8574 9.37921 37.1792 9.33398 36.4528 9.33398H30.3205C30.1694 9.33398 30.0259 9.36651 29.8976 9.42532C29.6147 9.55497 29.4047 9.81027 29.3537 10.1228L28.0491 18.0013L28.0117 18.231C28.0975 17.7124 28.5622 17.3308 29.1136 17.3308H31.409C35.9173 17.3308 39.4473 15.5849 40.4791 10.5347C40.5099 10.3852 40.5358 10.2398 40.559 10.0974C40.298 9.96532 40.0153 9.85237 39.7109 9.75614C39.6356 9.7323 39.5581 9.70935 39.4798 9.68708"
          fill="#00164C"
        />
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M29.353 10.1231C29.404 9.81053 29.614 9.55524 29.897 9.42648C30.0262 9.36744 30.1687 9.33492 30.3198 9.33492H36.4521C37.1785 9.33492 37.8567 9.38036 38.4756 9.47571C38.6525 9.50266 38.8242 9.53385 38.992 9.56883C39.1588 9.60447 39.3214 9.64435 39.4791 9.68801C39.5574 9.71029 39.635 9.73345 39.7109 9.7564C40.0153 9.85264 40.2983 9.96647 40.5592 10.0977C40.8662 8.23109 40.5567 6.96018 39.4983 5.80935C38.3313 4.54222 36.2253 4 33.5302 4H25.7062C25.1558 4 24.6861 4.38161 24.6011 4.90111L21.3423 24.5969C21.2781 24.9866 21.5933 25.3381 22.0054 25.3381H26.8356L29.353 10.1231"
          fill="#012F86"
        />
      </svg>
      <div
        class="flex flex-col justify-start items-start flex-grow relative gap-1"
      >
        <p
          class="flex-grow-0 flex-shrink-0 text-lg font-semibold text-left text-[#232323]"
        >
          Paypal
        </p>
        <p class="flex-grow-0 flex-shrink-0 text-sm text-left text-[#9a9a9a]">
          ganteng@mail.com
        </p>
      </div>
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
          d="M13.2594 3.60022L5.04936 12.2902C4.73936 12.6202 4.43936 13.2702 4.37936 13.7202L4.00936 16.9602C3.87936 18.1302 4.71936 18.9302 5.87936 18.7302L9.09936 18.1802C9.54936 18.1002 10.1794 17.7702 10.4894 17.4302L18.6994 8.74022C20.1194 7.24022 20.7594 5.53022 18.5494 3.44022C16.3494 1.37022 14.6794 2.10022 13.2594 3.60022Z"
          stroke="#9A9A9A"
          stroke-width="1.5"
          stroke-miterlimit="10"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M11.8906 5.0498C12.3206 7.8098 14.5606 9.9198 17.3406 10.1998"
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
  </div>
  <p
    class="flex-grow-0 flex-shrink-0 text-xs font-semibold text-left text-[#eb5842]"
  >
    Delete Account
  </p>
  <div
    class="flex justify-end items-start flex-grow-0 flex-shrink-0 w-[1208px] gap-3"
  >
    <div
      class="flex justify-center items-center flex-grow-0 flex-shrink-0 w-36 relative gap-2 p-4 bg-[#1f206c]"
    >
      <p
        class="flex-grow-0 flex-shrink-0 text-base font-medium text-center text-white"
      >
        Save Changes
      </p>
    </div>
  </div>
</div>

<style>
  p {
    font-family: var(--theme-font-family-base);
  }
</style>
