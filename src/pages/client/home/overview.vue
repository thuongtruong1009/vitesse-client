<script setup lang="ts">
const { t } = useI18n()

useHead({
  title: t('layout.client-home'),
})
</script>

<template>
  <div class="flex min-w-320 border-1 border-gray-600 text-white bg-black">
    <div class="logo-play flex items-center w-63 px-14">
      <img src="/public/assets/images/play-button/play-button-shape.png" class="w-9.4 h-10.5 cursor-pointer">
      <img src="/public/assets/images/play-button/play-button-click-area.png" class="w-30 h-8.5 cursor-pointer">
    </div>
    <div class="flex justify-between items-center">
      <ul class="navigation flex w-44 cursor-pointer font-semibold uppercase">
        <li>{{ t('tag.home') }}</li>
        <li>{{ t('tag.tft') }}</li>
        <li>{{ t('tag.clash') }}</li>
      </ul>
      <ul class="accessibility flex justify-end w-113 gap-10 cursor-pointer">
        <li><img src="/public/assets/images/header-icons/profile.png"></li>
        <li><img src="/public/assets/images/header-icons/collection.png"></li>
        <li><img src="/public/assets/images/header-icons/booty.png"></li>
        <li><img src="/public/assets/images/header-icons/shop.png"></li>
      </ul>
    </div>
    <div class="devide flex justify-center items-center w-10">
      <img src="/public/assets/images/header-icons/divider.png" width="1">
    </div>
    <div class="treasure grid justify-between items-center w-31 leading-none">
      <div class="treasure-point flex gap-2 font-semibold">
        <img src="/public/assets/images/header-icons/riot-points.png">88
      </div>
      <div class="treasure-blue flex gap-2 font-semibold">
        <img src="/public/assets/images/header-icons/blue-essence.png">2528
      </div>
    </div>
    <div class="profile flex justify-between items-center gap-3">
      <div class="avatar-rank flex justify-between items-center cursor-pointer">
        <img src="/public/assets/images/aside-icons/avatar-wrapper.png">
        <h6 class="absolute flex pl-6 pt-14">
          287
        </h6>
      </div>
      <div class="name-status grid justify-start items-center">
        <h2 class="font-semibold">
          {{ t('script.name') }}
        </h2>
        <h4 class="flex items-center gap-2 text-green-500">
          <img src="/public/assets/images/aside-icons/check.ico" class="border-2 border-green-300 rounded-full w-3.5 h-3.5">{{ t('script.status') }}
        </h4>
      </div>
    </div>
  </div>
</template>

<style lang="css">
.navigation >li {
  padding: 0 8px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.logo-play:after{
  content: "Play";
  position: absolute;
  align-self: center;
  padding-left: 75px;
  cursor: pointer;
}
</style>

<route lang="yaml">
meta:
  layout: client
</route>P
