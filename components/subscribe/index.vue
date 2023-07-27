<template>
  <section class="my-10 p-3 sm:px-16">
    <div
      class="grid grid-cols-3 gap-4 p-4 rounded-2xl items-center bg-gradient-to-r from-[#a1c0f9] via-white to-[#a1c0f9]"
    >
      <nuxt-img src="/images/right.png" alt="right-img" />
      <div class="space-y-3">
        <p class="capitalize text-center text-2xl text-[#1B1C57] font-semibold">
          Subscribe For More Info and update from Hounter
        </p>
        <div class="border bg-white rounded-full flex items-center p-1 text-xs">
          <div class="flex items-center px-4 py-2 w-full">
            <svg
              width="20"
              height="16"
              viewBox="0 0 20 16"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M17 0H3C2.20435 0 1.44129 0.316071 0.87868 0.87868C0.316071 1.44129 0 2.20435 0 3V13C0 13.7956 0.316071 14.5587 0.87868 15.1213C1.44129 15.6839 2.20435 16 3 16H17C17.7956 16 18.5587 15.6839 19.1213 15.1213C19.6839 14.5587 20 13.7956 20 13V3C20 2.20435 19.6839 1.44129 19.1213 0.87868C18.5587 0.316071 17.7956 0 17 0ZM17 2L10.5 6.47C10.348 6.55777 10.1755 6.60397 10 6.60397C9.82446 6.60397 9.65202 6.55777 9.5 6.47L3 2H17Z"
                fill="#3B82F6"
              />
            </svg>
            <input
              type="text"
              class="w-full bg-transparent px-2 outline-none border-0 placeholder:text-slate-400"
              placeholder="Your email here"
            />
          </div>
          <button
            class="block bg-[#10B981] rounded-full flex items-center py-3 justify-center text-white text-center w-1/2 text-xs"
          >
            Subsribe Now
          </button>
        </div>
      </div>
      <nuxt-img src="/images/left.png" alt="left-img" />
    </div>
  </section>
</template>
