<script setup lang="ts">
const { t } = useI18n()

useHead({
  title: t('layout.client-home'),
})
</script>

<template>
  <div class="flex min-w-320 border-1 border-gray-600 text-orange-100 bg-black max-h-min">
    <div class="left flex justify-center items-center w-2/6">
      <div class="logo-play flex items-center px-14">
        <img src="/assets/images/play-button/play-button-shape.png" class="w-9.4 h-10.5 cursor-pointer">
        <img src="/assets/images/play-button/play-button-click-area.png" class="w-30 h-8.5 cursor-pointer">
      </div>
      <div class="flex justify-between items-center">
        <ul class="navigation flex cursor-pointer font-semibold uppercase">
          <li>{{ t('tag.home') }}</li>
          <li>{{ t('tag.tft') }}</li>
          <li>{{ t('tag.clash') }}</li>
        </ul>
      </div>
    </div>
    <div class="right flex justify-evenly items-center w-4/6">
      <div class="accessibility flex justify-end items-center cursor-pointer w-6/12">
        <ul class="flex">
          <li><img src="/assets/images/header-icons/profile.png"></li>
          <li><img src="/assets/images/header-icons/collection.png"></li>
          <li><img src="/assets/images/header-icons/booty.png"></li>
          <li><img src="/assets/images/header-icons/shop.png"></li>
        </ul>
      </div>
      <div class="treasure-divider flex justify-between items-center pr-13 leading-none w-2/12">
        <img src="/assets/images/header-icons/divider.png">
        <div class="grid">
          <div class="point flex gap-2 font-semibold py-1">
            <img src="/assets/images/header-icons/riot-points.png">88
          </div>
          <div class="blue flex gap-2 font-semibold py-1">
            <img src="/assets/images/header-icons/blue-essence.png">2528
          </div>
        </div>
      </div>
      <div class="profile flex items-center w-3/12">
        <div class="avatar-rank flex justify-start items-center cursor-pointer pr-3">
          <img src="/assets/images/aside-icons/avatar-wrapper.png" class="z-1">
          <h6 class="absolute flex pl-6 pt-14 font-semibold text-opacity-5 z-2">
            287
          </h6>
          <img src="/assets/images/avatar/1.jpg" class="absolute rounded-full w-16 h-16 z-0">
        </div>
        <div class="name-status grid justify-start items-center">
          <h2 class="font-semibold text-left">
            {{ t('script.name') }}
          </h2>
          <h4 class="flex items-center gap-2 text-green-500">
            <img src="/assets/images/aside-icons/check.ico" class="border-2 border-green-300 rounded-full w-3.5 h-3.5">{{ t('script.status') }}
          </h4>
        </div>
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
.accessibility>ul>li{
  padding: 0 20px;
}
</style>

<route lang="yaml">
meta:
  layout: client
</route>P
