<script setup lang="ts">
const { t } = useI18n()
</script>

<template>
  <div class="grid bg-black min-w-72 h-20/24 text-orange-100 overflow-y-scroll">
    <div class="group-header flex justify-between items-center min-w-72 fixed z-2 bg-black">
      <h3 class="pl-2 font-semibold uppercase tracking-wider">
        {{ t('layout.social') }}
      </h3>
      <div class="extension flex justify-around w-3/6 cursor-pointer py-2">
        <img src="/public/assets/images/aside-icons/add-friend.png">
        <img src="/public/assets/images/aside-icons/add-folder.png">
        <img src="/public/assets/images/aside-icons/options.png">
        <img src="/public/assets/images/aside-icons/search.png">
      </div>
    </div>
    <div class="group-list grid mt-6">
      <ul class="flex justify-start items-center py-2">
        <li><img src="/public/assets/images/aside-icons/main-group-flag.png"></li>
        <li>XXXX</li>
        <li>Group main</li>
      </ul>
      <ul v-for="(i, index) in 3" :key="index" class="flex justify-start items-center py-2 cursor-pointer">
        <li><img src="/public/assets/images/aside-icons/group-flag.png"></li>
        <li>XXXX</li>
        <li>Group {{ i }}</li>
      </ul>
    </div>
    <div class="chat-header text-left font-semibold pl-2 uppercase">
      <h1 class="tracking-wider">
        {{ t('layout.general') }} (9/15)
      </h1>
    </div>
    <div class="chat-list grid">
      <div v-for="index in 14" :key="index" class="flex pl-2 py-2 cursor-pointer">
        <img class="border-2 border-orange-300 rounded-full w-13 h-13 mr-4" :src="`/public/assets/images/avatar/${index}.jpg`">
        <span class="status-icon w-3.2 h-3.2 top-8/12 right-7 rounded-full relative bg-green-600 border-3 border-solid border-green-400" />
        <div class="grid">
          <h5>Name {{ index }}</h5>
          <p class="text-green-500 ml-0">
            {{ t('layout.online') }}
          </p>
        </div>
      </div>
    </div>
    <ul class="tool flex justify-around min-w-72 h-1/15 fixed bottom-0 bg-black">
      <li>
        <img src="/public/assets/images/aside-icons/chat.png">
      </li>
      <li>
        <img src="/public/assets/images/aside-icons/missions.png">
      </li>
      <li>
        <img src="/public/assets/images/aside-icons/voice.png">
      </li>
      <li>
        v1.1
      </li>
      <li>
        <img src="/public/assets/images/aside-icons/bug.png">
      </li>
    </ul>
  </div>
</template>
<style lang="css">
.group-list>ul>li{
  padding: 0 7px;
}
.group-list>ul>li:nth-child(2){
  color: rgb(218, 170, 83);
}
.tool>li{
  display: flex;
  justify-content: center;
  align-items: center;
  border: 2px solid #785a28;
  width: 20%;
}
.tool>li:nth-child(4){
  border:none;
}
</style>
