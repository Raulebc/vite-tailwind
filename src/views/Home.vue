<script setup>
import Challenge from "../components/home/challenge.vue";
</script>

<template>
  <div class="text-white flex flex-col px-6 space-y-4">
    <div class="text-3xl font-bold pb-3">Dashboard</div>

    <div class="flex rounded-xl px-4 py-4 bg-slate-800">
      <div class="mr-3 rounded-full">
        <img
          src="https://i.pravatar.cc/150?img=3"
          class="rounded-full w-12 h-12"
        />
      </div>
      <div>
        <div class="font-bold">Jhon Wick</div>
        <div class="font-extralight">PuraSangre CrossFit</div>
      </div>
    </div>

    <Challenge />

    <div class="flex space-x-4 justify-between">
      <div class="space-y-4 w-1/2">
        <div class="bg-slate-800 rounded-xl py-3 px-3">
          <div class="text-xs font-semibold">Mobility Profile</div>
          <div class="flex justify-center py-3">
            <div
              class="bg-blue-500 bg-opacity-10 rounded-full flex items-center justify-center w-20 h-20"
            >
              <!-- we add the icon from the img folder -->
              <svg
                height="400px"
                width="400px"
                version="1.1"
                id="Capa_1"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                viewBox="0 0 61.858 61.858"
                xml:space="preserve"
                class="w-12 h-12 stroke-blue-400"
                stroke="currentColor"
                fill="currentColor"
                stroke-width="1.5"
              >
                <path
                  style="fill: transparent"
                  d="M50.097,0.014c-9.917,0.874-17.235,5.824-21.501,12.98c-2.859,3.584-8.57,14.526-10.647,20.254
              c-3.766,7.123-7.05,15.598-9.62,23.238c-1.571,4.672,5.483,7.72,7.063,3.027c1.922-5.716,4.244-11.896,6.868-17.631
              c2.604,5.828,5.25,11.637,8.091,17.354c2.202,4.438,8.828,0.546,6.634-3.877c-2.925-5.885-5.642-11.864-8.319-17.863
              c0.034-0.116,0.077-0.229,0.113-0.344c0.446,0.127,0.938,0.166,1.48,0.063c4.096-0.769,8.192-1.536,12.291-2.305
              c1.751-0.329,2.422-2.245,2.146-3.779c-0.828-4.597-3.447-7.795-6.707-10.821c-0.484-1.646-2.098-3.102-3.889-4.549
              c3.631-5.87,9.559-9.056,17.275-9.736C55.313,5.68,54.001-0.329,50.097,0.014z M35.173,26.143
              c1.013,1.054,1.875,2.163,2.526,3.447c-1.982,0.372-3.965,0.743-5.947,1.115C32.752,29.095,33.903,27.575,35.173,26.143z"
                />
                <circle
                  style="fill: transparent"
                  cx="43.653"
                  cy="15.635"
                  r="5.275"
                />
              </svg>
            </div>
          </div>
          <div class="text-xs font-extralight">
            <ul>
              <li>1. Shoulders</li>
              <li>2. Hips</li>
            </ul>
          </div>
        </div>
        <div class="bg-slate-800 rounded-xl py-3 px-3 space-y-3">
          <div class="text-xs font-semibold">Mobility time</div>
          <div class="text-blue-400 text-2xl font-light">121h28</div>
          <div class="text-xs font-extralight">
            <div>Since</div>
            <div class="text-blue-300">March 9, 2018</div>
          </div>
        </div>
      </div>
      <div class="w-1/2 rounded-xl bg-slate-800"></div>
    </div>
    <div class="rounded-xl px-4 py-4 bg-slate-800 space-y-2">
      <span class="font-bold text-gray-200">Smart reminders</span>
      <div class="flex space-x-3 items-center">
        <div class="w-20 flex justify-center mx-">
          <div
            class="bg-blue-500 bg-opacity-10 rounded-full flex items-center justify-center w-20 h-20"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              strokeWidth="{1.5}"
              stroke="currentColor"
              class="w-12 h-12 text-blue-400"
            >
              <path
                strokeLinecap="round"
                strokeLinejoin="round"
                d="M14.857 17.082a23.848 23.848 0 005.454-1.31A8.967 8.967 0 0118 9.75v-.7V9A6 6 0 006 9v.75a8.967 8.967 0 01-2.312 6.022c1.733.64 3.56 1.085 5.455 1.31m5.714 0a24.255 24.255 0 01-5.714 0m5.714 0a3 3 0 11-5.714 0"
              />
            </svg>
          </div>
        </div>

        <div class="flex flex-col space-y-1">
          <span class="text-sm/[16px] text-blue-400 opacity-80"
            >Improve your consistency</span
          >
          <span class="text-sm/[16px] md:text-base text-gray-200">
            Configure your own remiders to help you to perform for the long
            term.
          </span>
        </div>
      </div>
    </div>
  </div>
</template>
