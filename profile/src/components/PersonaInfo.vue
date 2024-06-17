<!-- 包括头像、昵称 帖子数、粉丝数、关注数-->
<template>
  <div class="info-card">
    
    <div class="profile-image"></div>
    <div class="sign">sign:Hello Every one!</div>
    <div class="name">
      <div class="username">用户名Yunshiro</div>
      <div class="nickname">昵称Yun</div>
    </div>
    
    <div class="detail">
      <ul>
        <li>帖子数{{ a }}</li>
        <li>粉丝数{{ a }}</li>
        <li>关注数{{ a }}</li>
      </ul>
    </div>
  </div>
</template>

<script setup lang='ts'>
import { ref } from 'vue'

let a = ref(0)
</script>

<style scoped>
.info-card {
  border: 2px solid;
  width: 500px;
  height: 200px;
  margin: 0;
  position: absolute;

}

.profile-image {
  border-radius: 50%;
  border: 1px solid;
  height: 140px;
  width: 140px;
  background-color: pink;
  
  position: absolute;
  top: 14px;
  left: 10px;
}

.sign {
  position: absolute;
  top: 80px;
  left: 170px;
}

.detail ul {
  list-style: none;
  display: flex;
  position: absolute;
  top: 140px;
  left: 170px;

  margin: 0;
  padding: 0;
}

.detail ul li {
  margin-right: 40px;
  margin-left: 0;
  padding: 0;
  width: 80px;
}

.name {
  position: absolute;
  left: 170px;
  top: 14px;
  margin: 0;
  padding: 0;
}

.name .username {
  margin-bottom: 20px;
}
</style>