<template>
	<div class="flex flex-col rounded-xl px-4 py-4 bg-slate-800 space-y-3">
    <div class="flex justify-between w-full">
      <div class="space-y-4">
        <div class="text-xs font-bold">GOWOD Challenge</div>
        <div class="flex items-end space-x-2">
          <span class="text-3xl text-blue-400">2h25</span>
          <span>/</span>
          <span>7h00</span>
        </div>
      </div>
      <div class="bg-blue-500 bg-opacity-10  rounded-full flex items-center justify-center w-20 h-20">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" strokeWidth={1.5} stroke="currentColor" class="w-12 h-12 text-blue-400">
          <path strokeLinecap="round" strokeLinejoin="round" d="M16.5 18.75h-9m9 0a3 3 0 013 3h-15a3 3 0 013-3m9 0v-3.375c0-.621-.503-1.125-1.125-1.125h-.871M7.5 18.75v-3.375c0-.621.504-1.125 1.125-1.125h.872m5.007 0H9.497m5.007 0a7.454 7.454 0 01-.982-3.172M9.497 14.25a7.454 7.454 0 00.981-3.172M5.25 4.236c-.982.143-1.954.317-2.916.52A6.003 6.003 0 007.73 9.728M5.25 4.236V4.5c0 2.108.966 3.99 2.48 5.228M5.25 4.236V2.721C7.456 2.41 9.71 2.25 12 2.25c2.291 0 4.545.16 6.75.47v1.516M7.73 9.728a6.726 6.726 0 002.748 1.35m8.272-6.842V4.5c0 2.108-.966 3.99-2.48 5.228m2.48-5.492a46.32 46.32 0 012.916.52 6.003 6.003 0 01-5.395 4.972m0 0a6.726 6.726 0 01-2.749 1.35m0 0a6.772 6.772 0 01-3.044 0" />
        </svg>
      </div>
    </div>
    <div class="space-y-2">
      <div class="w-full bg-gray-900 rounded-full h-2.5 dark:bg-gray-700">
        <div class="bg-blue-400 h-2.5 rounded-full" style="width: 45%"></div>
      </div>
      <div class="flex justify-between text-xs text-gray-300">
        <div>Time remaining</div>
        <div>1 day</div>
      </div>
    </div>
  </div>
</template>