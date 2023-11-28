<template>
  <div class="container">
    <div class="row mt-5">
      <div class="col-xs-3 col-sm-3 col-md-3 col-lg-3">
        <div>
          <ul>
            <li class="menu-block">Моя страница</li>
            <li class="menu-block">Новости</li>
            <li class="menu-block">Мессенджер</li>
            <li class="menu-block">Друзья</li>
          </ul>
        </div>
      </div>
      <div class="col-xs-9 col-sm-9 col-md-9 col-lg-9">
        <div class="page-header">
          <div style="margin: 20px; font-size: 20px; font-weight: bold">
            <img src="/img/avatar.jpg" style="border-radius: 0.5rem;"/>
            Имя Фамилия
          </div>
          <div class="settingsbox">
            Настройки
          </div>
        </div>
        <div class="row page-body mt-4" style="margin: 0px">
          <div class="col-xs-8 col-sm-8 col-md-8 col-lg-8 page-feed">
            Посты
          </div>
          <div class="col-xs-4 col-sm-4 col-md-4 col-lg-4 page-friends">
            <div class="mb-2">
              Друзья
            </div>
            <div style="display: flex; width: 50px; height: 50px; ">
              <img src="/img/avatar.jpg" style="border-radius: 0.5rem;" class="center-img"/>
              <img src="/img/avatar.jpg" style="border-radius: 0.5rem;" class="center-img"/>
              <img src="/img/avatar.jpg" style="border-radius: 0.5rem;" class="center-img"/>
              <img src="/img/avatar.jpg" style="border-radius: 0.5rem;" class="center-img"/>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "PageView"
}
</script>

<style scoped>

</style>