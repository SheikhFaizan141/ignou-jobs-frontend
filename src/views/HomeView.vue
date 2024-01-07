<script setup>
import AppButton from '@/components/AppButton.vue';

</script>

<template>
  <div class="jobsearch-box py-3 flex  justify-center border-b border-b-gray-200">
    <div class="search-bar flex items-center justify-center border border-black rounded p-2 shadow shadow-slate-500 ">
      <form class="flex gap-1 items-center ">
        <div>
          <span class="search-icon">
            <i>🔍</i>
          </span>
          <input
            type="search"
            placeholder="Job title or company"
            class="p-1 rounded"
          >
        </div>
        <AppButton
          type="submit"
          class=""
        >
          Search
        </AppButton>
      </form>
    </div>
  </div>
  <main class="px-4 py-2">
    <div class="listing-container grid grid-rows-5 grid-cols-3 gap-2">


      <div
        v-for="n in  15"
        class="listing-card border rounded shadow shadow-slate-300 p-3 cursor-pointer"
      >
        <div class="listing-heading mb-1 ">
          <div class="mb-1 tag tag-new px-1 text-sm text-purple-700 font-medium border inline-block rounded ">New</div>
          <h2 class="text-xl font-bold">Senior Accountant</h2>
        </div>
        <div class="listing-location flex flex-col mb-1">
          <span class="listing-name">Tata Consultancy</span>
          <span class="listing-location">Bengaluru, Karnataka</span>
        </div>

        <div class="listing-metadata-box flex flex-wrap gap-1 text-sm mb-1">
          <div class="metadata bg-gray-300 rounded-sm px-1 py-0.5">
            $4,00 - 6,00$ a day
          </div>
          <div class="metadata bg-gray-300 rounded-sm px-1 py-0.5">
            Part-Time
          </div>
          <div class="metadata bg-gray-300 rounded-sm px-1 py-0.5">
            Day Shift
          </div>
        </div>

        <div class="listing-discription py-2 text-sm text-gray-600">
          <ol
            class="list-inside"
            style="list-style-type: circle;"
          >
            <li class="list-group-item">Cras justo odio</li>
            <li class="list-group-item">Cras justo odio</li>
            <li class="list-group-item">Cras justo odio</li>
          </ol>
        </div>

        <div class="listing-btn mb-1">
          <AppButton class="px-10 mb-1">Apply</AppButton>
        </div>
        <div class="posted text-xs font-light ">Posted 1 day ago</div>
      </div>

    </div>

    <div class="pagenation flex justify-center py-2">
    <nav aria-label="Page navigation example">
      <ul class="inline-flex -space-x-px text-sm">
        <li>
          <a
            href="#"
            class="flex items-center justify-center px-3 h-8 ms-0 leading-tight text-gray-500 bg-white border border-e-0 border-gray-300 rounded-s-lg hover:bg-gray-100 hover:text-gray-700 dark:bg-gray-800 dark:border-gray-700 dark:text-gray-400 dark:hover:bg-gray-700 dark:hover:text-white"
          >Previous</a>
        </li>
        <li>
          <a
            href="#"
            class="flex items-center justify-center px-3 h-8 leading-tight text-gray-500 bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700 dark:bg-gray-800 dark:border-gray-700 dark:text-gray-400 dark:hover:bg-gray-700 dark:hover:text-white"
          >1</a>
        </li>
        <li>
          <a
            href="#"
            class="flex items-center justify-center px-3 h-8 leading-tight text-gray-500 bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700 dark:bg-gray-800 dark:border-gray-700 dark:text-gray-400 dark:hover:bg-gray-700 dark:hover:text-white"
          >2</a>
        </li>
        <li>
          <a
            href="#"
            aria-current="page"
            class="flex items-center justify-center px-3 h-8 text-blue-600 border border-gray-300 bg-blue-50 hover:bg-blue-100 hover:text-blue-700 dark:border-gray-700 dark:bg-gray-700 dark:text-white"
          >3</a>
        </li>
        <li>
          <a
            href="#"
            class="flex items-center justify-center px-3 h-8 leading-tight text-gray-500 bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700 dark:bg-gray-800 dark:border-gray-700 dark:text-gray-400 dark:hover:bg-gray-700 dark:hover:text-white"
          >4</a>
        </li>
        <li>
          <a
            href="#"
            class="flex items-center justify-center px-3 h-8 leading-tight text-gray-500 bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700 dark:bg-gray-800 dark:border-gray-700 dark:text-gray-400 dark:hover:bg-gray-700 dark:hover:text-white"
          >5</a>
        </li>
        <li>
          <a
            href="#"
            class="flex items-center justify-center px-3 h-8 leading-tight text-gray-500 bg-white border border-gray-300 rounded-e-lg hover:bg-gray-100 hover:text-gray-700 dark:bg-gray-800 dark:border-gray-700 dark:text-gray-400 dark:hover:bg-gray-700 dark:hover:text-white"
          >Next</a>
        </li>
      </ul>
    </nav>
  </div>
  </main>
</template>
