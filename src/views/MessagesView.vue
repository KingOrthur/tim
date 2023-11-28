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
      <div class="col-xs-9 col-sm-9 col-md-9 col-lg-9 chat-list" style="display: flex">
        <div class="col-xs-3 col-sm-3 col-md-3 col-lg-3 mt-3 mb-3">
          <div class="chat">
              Поиск
          </div>
          <div class="chat">
            <img src="/img/avatar.jpg" width="50" height="35"/>
            <div style="margin-left: 10px">
              Андрей Андреев
            </div>
          </div>
          <div class="chat">
            <img src="/img/avatar.jpg" width="50" height="35"/>
            <div style="margin-left: 10px">
              Максим Максимов
            </div>
          </div>
          <div class="chat">
            <img src="/img/avatar.jpg" width="50" height="35"/>
            <div style="margin-left: 10px">
              Олег Олегов
            </div>
          </div>
          <div class="chat">
            <img src="/img/avatar.jpg" width="50" height="35"/>
            <div style="margin-left: 10px">
              Никита Никитов
            </div>
          </div>
          <div class="chat">
            <img src="/img/avatar.jpg" width="50" height="35"/>
            <div style="margin-left: 10px">
              Денис Денисов
            </div>
          </div>
          <div class="chat">
            <img src="/img/avatar.jpg" width="50" height="35"/>
            <div style="margin-left: 10px">
              Саша Саша
            </div>
          </div>
          <div class="chat">
            <img src="/img/avatar.jpg" width="50" height="35"/>
            <div style="margin-left: 10px">
              Константин
            </div>
          </div>
        </div>
        <div class="col-xs-9 col-sm-9 col-md-9 col-lg-9 mt-3 mb-3" style="position:relative; padding-bottom:500px;">
          <div class="chat-top" style="justify-content: space-between">
            <div>Название чата</div>
            <div>Поиск</div>
          </div>
          <div>
            текст
          </div>
          <div>
            <div class="input-group mb-3">
              <input type="text" class="form-control" placeholder="Напишите сообщение" aria-label="Username" aria-describedby="basic-addon1">
            </div>
          </div>
        </div>
      </div>

    </div>
  </div>
</template>

<script>
import Chat from "@/components/Chat.vue";

export default {
  name: "MessagesView",
  components: {Chat}
}
</script>

<style scoped>


.chat{
  border-top: 1px solid gray;
  font-size: 12px;
  display: flex;
  padding: 5px;
  text-align: left;
}

.chat:hover {
  background-color: lightgray;
}
.chat-top{
  font-size: 12px;
  display:flex;
  margin-left: 30px;
  padding: 5px;
  text-align: left;
  border-bottom: 1px solid gray;

}
</style>