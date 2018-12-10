<template>
  <div class="container container--centered">
    <from action="" class="urlfrom">
      <input type="url" placeholder="请输入你的链接..." class="urlfrom__input">
    </from>

    <div class="result">
      <div class="result__details">
        <div class="result__original">
          原链接：<span>https://www.baidu.com</span>
        </div>
        <a href="" target="_blank" class="result__url">https://www.baidu.com</a>
        <a href="" class="result__stats">获取短链接</a>
      </div>
      <button class="button button--yellow">复制链接</button>
    </div>

    <!--<div class="notice">-->
    <!--ceshi-->
    <!--</div>-->

    <!--<div class="notice">-->
    <!--</div>-->

  </div>
</template>

<style lang="scss">
  .urlfrom {
    width: 100%;
    margin-bottom: 40px;

    &__input {
      font: inherit;
      font-size: 1.2em;
      padding: 20px;
      width: 100%;
      border: 0;
      outline: none;
      border-radius: 3px;
      box-shadow: 0 0 50px rgba(#fff, .1);
    }
  }

  .notice {
    color: #fff;
    font-size: 1.1em;
    font-weight: 500;
  }

  .result {

    width: 100%;
    text-align: center;

    &__details {
      color: #fff;
      font-size: 1.4em;
    }

    &__stats {
      display: block;
      color: #fff;
      font-size: .9em;
      margin-bottom: 20px;
    }

    &__original {
      opacity: 0.5;
      margin-bottom: 5px;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;

      span {
        display: inline-block;
        max-width: 300px;
        overflow: hidden;
        white-space: nowrap;
        text-overflow: ellipsis;
        margin-right: 8px;
      }
    }

    &__url {
      display: block;
      margin-bottom: 20px;
      color: #fff;
    }

    @media (min-width: 736px) {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: center;

      &__stats {
        margin-bottom: 0;
      }

      &__details {
        margin-right: 40px;
      }
    }
  }
</style>
