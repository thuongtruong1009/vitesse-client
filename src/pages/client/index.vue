<template>
  <div class="flex w-screen border-1 border-gray-600 text-white">
    <div class="logo-play inline-flex justify-evenly items-center w-62">
      <img src="/public/assets/images/play-button/play-button-shape.png">
      <img src="/public/assets/images/play-button/play-button-click-area.png">
    </div>
    <div class="inline-flex justify-between items-center">
      <ul class="navigation flex w-44 gap-3">
        <li>HOME</li>
        <li>TFT</li>
        <li>CLASH</li>
      </ul>
      <ul class="accessibility flex justify-end w-113 gap-8">
        <li><img src="/public/assets/images/header-icons/profile.png"></li>
        <li><img src="/public/assets/images/header-icons/collection.png"></li>
        <li><img src="/public/assets/images/header-icons/booty.png"></li>
        <li><img src="/public/assets/images/header-icons/shop.png"></li>
      </ul>
    </div>
    <div class="devide flex justify-center align-center w-10">
      <img src="/public/assets/images/header-icons/divider.png">
    </div>
    <div class="treasure grid justify-between items-center w-31">
      <img src="/public/assets/images/header-icons/riot-points.png">
      <img src="/public/assets/images/header-icons/blue-essence.png">
    </div>
    <div class="profile flex justify-between items-center gap-3">
      <div class="avatar-rank flex justify-between items-center">
        <img src="/public/assets/images/aside-icons/avatar-wrapper.png">
      </div>
      <div class="name-status grid justify-start items-center">
        <h2>Name</h2>
        <h4 class="flex items-center gap-2 text-green-500">
          <img src="/public/assets/images/aside-icons/check.ico" class="border-2 border-green-300 rounded-full w-3.5 h-3.5">online
        </h4>
      </div>
    </div>
  </div>
</template>

<route lang="yaml">
meta:
  layout: client
</route>
