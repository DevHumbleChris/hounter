<script setup>
const houses = useState("houses", () => {
  return [
    {
      name: "Roselands House",
      price: "$ 35.000.000",
      imgURL: "/images/featured/Roselands.jpg",
      owner: {
        imgUrl: "/images/featured/Dianne.jpg",
        name: "Dianne Russell",
        address: "Manchester, Kentucky",
      },
      tag: {
        icon: "/images/featured/fire.png",
        name: "Popular",
      },
    },
    {
      name: "Woodlandside",
      price: "$ 20.000.000",
      imgURL: "/images/featured/Woodlandside.jpg",
      owner: {
        imgUrl: "/images/featured/RobertFox.jpg",
        name: "Robert Fox",
        address: "Dr. San Jose, South Dakota",
      },
      tag: {
        icon: "/images/featured/NewHouse.png",
        name: "New House",
      },
    },
    {
      name: "The Old Lighthouse",
      price: "$ 44.000.000",
      imgURL: "/images/featured/TheOldLighthouse.jpg",
      owner: {
        imgUrl: "/images/featured/RonaldRichards.jpg",
        name: "Ronald Richards",
        address: "Santa Ana, Illinois",
      },
      tag: {
        icon: "/images/featured/wallet.png",
        name: "Best Deals",
      },
    },
    {
      name: "Cosmo's House",
      price: "$ 22.000.000",
      imgURL: "/images/featured/Cosmo'sHouse.jpg",
      owner: {
        imgUrl: "/images/featured/JennyWilson.jpg",
        name: "Jenny Wilson",
        address: "Preston Rd. Inglewood, Maine 98380",
      },
      tag: {
        icon: "/images/featured/fire.png",
        name: "Popular",
      },
    },
  ];
});
</script>

<template>
  <section class="my-20 p-5 sm:px-16">
    <div class="space-y-6">
      <div
        class="flex flex-col gap-y-3 sm:flex-row sm:items-center justify-between"
      >
        <div>
          <div class="flex items-center space-x-3">
            <svg
              width="32"
              height="1"
              viewBox="0 0 32 1"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <rect width="32" height="1" fill="#F59E0B" />
            </svg>

            <p class="text-[#F59E0B] text-[0.7rem]">Our Recommendation</p>
          </div>
          <p class="text-[#1B1C57] font-semibold text-2xl">Featured House</p>
        </div>
        <div class="flex items-center justify-between space-x-5">
          <button
            aria-label="House"
            class="flex items-center space-x-2 border bg-[#D1FAE5] text-[#10B981] text-semibold px-4 py-2 bg-[#96CBE5] rounded-full"
          >
            <svg
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M21 10.8319V19.5C20.9998 19.7719 20.9262 20.0386 20.7868 20.272C20.6475 20.5054 20.4476 20.6968 20.2084 20.8259C19.9916 20.9432 19.7485 21.0031 19.5021 20.9999H14.9967C14.7978 20.9999 14.607 20.9209 14.4664 20.7803C14.3257 20.6396 14.2467 20.4488 14.2467 20.2499V15.7493C14.2467 15.5504 14.1677 15.3596 14.0271 15.2189C13.8864 15.0783 13.6956 14.9993 13.4967 14.9993H10.4967C10.2978 14.9993 10.107 15.0783 9.9664 15.2189C9.82574 15.3596 9.74673 15.5504 9.74673 15.7493V20.2499C9.74673 20.4488 9.66771 20.6396 9.52706 20.7803C9.3864 20.9209 9.19564 20.9999 8.99673 20.9999H4.5002C4.28754 21.0005 4.07723 20.9556 3.88335 20.8682C3.68948 20.7808 3.51651 20.653 3.37604 20.4934C3.12946 20.2082 2.99571 19.8427 3.00001 19.4657V10.8318C3.00017 10.6228 3.04392 10.4162 3.12846 10.225C3.21299 10.0339 3.33646 9.86251 3.49098 9.7218L10.9903 2.90308C11.2658 2.65075 11.6258 2.51078 11.9994 2.51074C12.3729 2.51071 12.733 2.65062 13.0085 2.90289L20.5091 9.72189C20.6636 9.86263 20.787 10.034 20.8716 10.2252C20.9561 10.4163 20.9998 10.6229 21 10.8319Z"
                fill="#10B981"
              />
            </svg>
            <p>House</p>
          </button>
          <button
            aria-label="Villa"
            class="flex items-center space-x-2 border bg-transparent text-semibold px-4 py-2 bg-[#96CBE5] text-[#888B97] rounded-full"
          >
            <svg
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M7 20.9999H4C3.45 20.9999 3 20.5499 3 19.9999V8.68994C3 8.26994 3.25 7.89994 3.64 7.74994L14.64 3.51994C14.7921 3.46126 14.9561 3.44064 15.118 3.45986C15.2798 3.47909 15.4345 3.53758 15.5686 3.63025C15.7027 3.72292 15.8121 3.84696 15.8873 3.99156C15.9624 4.13617 16.0012 4.29696 16 4.45994V9.99994H8C7.45 9.99994 7 10.4499 7 10.9999V20.9999ZM17 11.9999H10C9.45 11.9999 9 12.4499 9 12.9999V19.9999C9 20.5499 9.45 20.9999 10 20.9999H14V16.9999C14 16.4499 14.45 15.9999 15 15.9999C15.55 15.9999 16 16.4499 16 16.9999V20.9999H20C20.55 20.9999 21 20.5499 21 19.9999V11.9999C21 10.8999 20.1 9.99994 19 9.99994C17.9 9.99994 17 10.8999 17 11.9999Z"
                fill="#888B97"
              />
            </svg>

            <p>Villa</p>
          </button>
          <button
            aria-label="Apartment"
            class="flex items-center space-x-2 border bg-transparent text-semibold px-4 py-2 bg-[#96CBE5] text-[#888B97] rounded-full"
          >
            <svg
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M17 11V5C17 3.9 16.1 3 15 3H9C7.9 3 7 3.9 7 5V7H5C3.9 7 3 7.9 3 9V19C3 20.1 3.9 21 5 21H11V17H13V21H19C20.1 21 21 20.1 21 19V13C21 11.9 20.1 11 19 11H17ZM7 19H5V17H7V19ZM7 15H5V13H7V15ZM7 11H5V9H7V11ZM11 15H9V13H11V15ZM11 11H9V9H11V11ZM11 7H9V5H11V7ZM15 15H13V13H15V15ZM15 11H13V9H15V11ZM15 7H13V5H15V7ZM19 19H17V17H19V19ZM19 15H17V13H19V15Z"
                fill="#888B97"
              />
            </svg>
            <p>Apartment</p>
          </button>
        </div>
        <div class="flex items-center justify-between space-x-1">
          <button
            aria-label="chevron-left"
            class="flex items-center space-x-2 border bg-[#E0E3EB] text-[#10B981] text-semibold px-4 py-2 bg-[#96CBE5] rounded-full"
          >
            <svg
              width="28"
              height="28"
              viewBox="0 0 28 28"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M17.5078 22.1645C17.7781 22.165 18.04 22.0703 18.2482 21.8967C18.3653 21.799 18.4622 21.679 18.5331 21.5436C18.6041 21.4081 18.6478 21.2599 18.6618 21.1075C18.6758 20.955 18.6597 20.8012 18.6145 20.655C18.5694 20.5088 18.496 20.373 18.3986 20.2554L13.2158 14.0159L18.2135 7.76475C18.3096 7.64567 18.3813 7.50867 18.4246 7.3616C18.4679 7.21453 18.4819 7.0603 18.4658 6.90777C18.4497 6.75524 18.4038 6.60742 18.3307 6.47281C18.2576 6.3382 18.1588 6.21945 18.0399 6.12339C17.9202 6.01741 17.7801 5.93748 17.6282 5.8886C17.4764 5.83972 17.3161 5.82295 17.1575 5.83935C16.9989 5.85574 16.8454 5.90495 16.7066 5.98388C16.5678 6.0628 16.4467 6.16975 16.3509 6.298L10.7632 13.2825C10.593 13.4908 10.5 13.7521 10.5 14.0217C10.5 14.2913 10.593 14.5526 10.7632 14.7609L16.5476 21.7454C16.6636 21.8863 16.811 21.9976 16.9779 22.0705C17.1447 22.1433 17.3263 22.1755 17.5078 22.1645Z"
                fill="#3C4563"
              />
            </svg>
          </button>
          <button
            aria-label="chevron-right"
            class="flex items-center space-x-2 border bg-[#10B981] text-semibold px-4 py-2 rounded-full"
          >
            <svg
              width="28"
              height="28"
              viewBox="0 0 28 28"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M11.6589 5.83552C11.3886 5.83499 11.1266 5.92971 10.9185 6.10326C10.8014 6.20098 10.7045 6.321 10.6336 6.45644C10.5626 6.59188 10.5189 6.74007 10.5049 6.89254C10.4909 7.04501 10.507 7.19875 10.5521 7.34496C10.5973 7.49118 10.6707 7.62699 10.7681 7.74462L15.9509 13.9841L10.9532 20.2353C10.8571 20.3543 10.7854 20.4913 10.7421 20.6384C10.6988 20.7855 10.6848 20.9397 10.7009 21.0922C10.717 21.2448 10.7629 21.3926 10.836 21.5272C10.9091 21.6618 11.0079 21.7806 11.1267 21.8766C11.2464 21.9826 11.3866 22.0625 11.5385 22.1114C11.6903 22.1603 11.8506 22.177 12.0092 22.1607C12.1678 22.1443 12.3213 22.0951 12.4601 22.0161C12.5989 21.9372 12.72 21.8303 12.8158 21.702L18.4035 14.7175C18.5736 14.5092 18.6667 14.2479 18.6667 13.9783C18.6667 13.7087 18.5736 13.4474 18.4035 13.2391L12.6191 6.25459C12.5031 6.11371 12.3556 6.00235 12.1888 5.92954C12.022 5.85673 11.8404 5.82452 11.6589 5.83552Z"
                fill="white"
              />
            </svg>
          </button>
        </div>
      </div>
      <div class="flex items-center space-x-8 overflow-x-scroll scrollbar-hide">
        <div
          v-for="(house, index) in houses"
          :key="index"
          class="space-y-3 shrink-0"
        >
          <div class="relative">
            <nuxt-img
              :src="house.imgURL"
              :alt="house.imgURL"
              class="w-full h-72 object-cover"
              format="webp"
              quality="80"
              width="340"
              height="382"
            />
            <div
              class="absolute bottom-4 left-4 px-3 py-2 rounded-full flex items-center space-x-1"
              :class="{
                'bg-[#FEE2E2]': house.tag.name === 'Popular',
                'bg-[#DBEAFE]': house.tag.name === 'New House',
                'bg-[#D1FAE5]': house.tag.name === 'Best Deals',
              }"
            >
              <nuxt-img
                :src="house.tag.icon"
                :alt="house.tag.name"
                format="webp"
                quality="80"
                width="16"
                height="16"
              />
              <p
                class="text-[0.6rem] mt-[2px]"
                :class="{
                  'text-[#EF4444]': house.tag.name === 'Popular',
                  'text-[#1D4ED8]': house.tag.name === 'New House',
                  'text-[#047857]': house.tag.name === 'Best Deals',
                }"
              >
                {{ house.tag.name }}
              </p>
            </div>
          </div>
          <div>
            <p class="text-[#0E1735] font-medium">{{ house.name }}</p>
            <p class="text-[#3C4563] text-sm">{{ house.price }}</p>
          </div>
          <div class="flex items-center space-x-2">
            <nuxt-img
              :src="house.owner.imgUrl"
              :alt="house.owner.name"
              class="rounded-full w-8 h-8"
              format="webp"
              quality="80"
              width="40"
              height="40"
            />
            <div>
              <p class="text-[0.8rem] font-medium text-[#0E1735]">
                {{ house.owner.name }}
              </p>
              <p class="text-[#888B97] text-[0.6rem]">
                {{ house.owner.address }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
