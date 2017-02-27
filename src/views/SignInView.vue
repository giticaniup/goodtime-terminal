<template>
  <scroller class="wrapper">
    <div class="title-div">
      <text class="title-text">微信报名</text>
    </div>
    <div class="page-head">
      <image class="title-bg" resize="cover" src="https://img.alicdn.com/tps/TB1dX5NOFXXXXc6XFXXXXXXXXXX-750-202.png"></image>
    </div>
    <div class="article">
      <text class="content-title">登山</text>
      <text class="article-paragraph">春暖花开时，正是登山日</text>
      <text class="article-paragraph">春暖花开时，正是登山日</text>  
      <a href="www.baidu.com"><text style="color: orange" class="article-paragraph">更多信息请点击</text></a>
    </div>
    <div style="align-items: center;">
       <image class="contain" src="http://192.168.16.102/files/time.jpg"></image>
       <text class="content-title">Joyce</text>
    </div>
    <div class="sign-div">
      <button class="sign-in"><text class="sign-text">点击报名</text></button>
    </div>
</scroller>
</template>
<style>
  .title-div{
    width: 750px;
    height: 100px;
    background-color:#3E3E40;
    justify-content: center;
    align-items: center;
  }
  .page-head {
    width: 750px;
    height: 200px;
  }
  .title-bg {
    width: 750px;
    height: 200px;
  }
  .title-box {
    width: 750px;
    height: 200px;
    justify-content: center;
    align-items: center;
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
  }
  .title {
    color: #ffffff;
    font-size: 32px;
    font-weight: bold;
  }
  .article {
    padding: 40px;
    justify-content: center;
    align-items: center;
  }
  .article-paragraph{
    margin-top: 15px;
  }
  .sign-div{
    justify-content: center;
    align-items: center;
  }
  .sign-in{
    margin-top: 30px;
    width: 400px;
    height: 100px;
    font: 50px;
    background-color: orange;
    border-radius: 15px;
  }
  .sign-text{
    text-align: center;
    vertical-align: middle;
    color: white;
    font-size: 70px;
  }
  .title-text{
    text-align: center;
    vertical-align: middle;
    color: white;
    font-size: 50px;
    font-weight: bold;
  }
  .contain {
    width:200px;
    height:200px;
    border-width: 1;
  }
  .content-title{
    font-size: 40px;
    color: black;
    font-weight: bold;
    text-align: center;
    vertical-align: middle;
  }
</style>