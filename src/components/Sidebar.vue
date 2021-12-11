<template>
  <div class="grid bg-black min-w-72 text-orange-100 uppercase">
    <div class="group-header flex justify-between items-center">
      <h4 class="pl-2 font-semibold">
        Social
      </h4>
      <div class="extension flex justify-around w-3/6">
        <img src="/public/assets/images/aside-icons/add-friend.png">
        <img src="/public/assets/images/aside-icons/add-folder.png">
        <img src="/public/assets/images/aside-icons/options.png">
        <img src="/public/assets/images/aside-icons/search.png">
      </div>
    </div>
    <div class="group-list grid">
      <ul>
        <li><img src="/public/assets/images/aside-icons/main-group-flag.png"></li>
        <li>XXXX</li>
        <li>Group 1</li>
      </ul>
      <ul>
        <li><img src="/public/assets/images/aside-icons/group-flag.png"></li>
        <li>XXXX</li>
        <li>Group 2</li>
      </ul>
      <ul>
        <li><img src="/public/assets/images/aside-icons/main-group-flag.png"></li>
        <li>XXXX</li>
        <li>Group 3</li>
      </ul>
    </div>
    <div class="chat-header text-left font-semibold pl-2">
      <h1>General (9/15)</h1>
    </div>
    <div class="chat-list grid">
      <div class="flex pl-2 py-2">
        <img class="border-2 border-orange-300 rounded-full w-13 h-13 mr-3" src="/public/assets/images/avatar/1.jpg">
        <div class="grid">
          <h5>Yasou</h5>
          <p>online</p>
        </div>
      </div>
    </div>
  </div>
</template>
<style lang="css">
.group-list>ul{
  display: flex;
  justify-content: start;
  align-items: center;
  padding: 5px 0;
}
.group-list>ul>li{
  padding: 0 7px;
}
.group-list>ul>li:nth-child(2){
  color: rgb(218, 170, 83);
}
</style>
