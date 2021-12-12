<template>
  <main class="text-center text-gray-700 dark:text-gray-200 min-w-screen-lg h-screen overflow-hidden">
    <router-view class="h-3/24" />
    <div class="flex justify-between min-w-screen h-21/24">
      <div class="flex items-center w-10/12">
        [Client Home Overview layout]
      </div>
      <Sidebar class="w-2/12" />
    </div>
  </main>
</template>

<style lang="css">
::-webkit-scrollbar {
  width: 4px;
  height: 4px;
}
::-webkit-scrollbar,
::-webkit-scrollbar-track {
  background: transparent;
}
::-webkit-scrollbar-thumb {
  background: #785a28;
  border-radius: 300px;
}</style>
