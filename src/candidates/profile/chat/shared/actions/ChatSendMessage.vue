<template>
  <form class="chat-message-field">
    <textarea class="chat-message-field__input" placeholder="Say something..."></textarea>
    <button class="chat-message-field__btn" type="button">
      <svg class="chat-message-field__btn-icon">
        <use xlink:href="#arrow"></use>
      </svg>
    </button>
  </form>
</template>

<script>
export default {};
</script>

<style lang="postcss" scoped>
  .chat-message-field {
    display: flex;
    align-items: center;
    width: 100%;
    padding: 0 35px;
    box-sizing: border-box;
  }
  .chat-message-field__input {
    flex: 1;
    display: block;
    height: 48px;
    margin-right: 25px;
    padding: 15px 25px;
    font-size: 14px;
    line-height: 16px;
    color: #90A4AE;
    border-radius: 24px;
    border: 1px solid #CFD8DC;
    box-sizing: border-box;
    resize: none;
    outline: none;
    &::placeholder {
      font-size: 14px;
      line-height: 16px;
      color: #CFD8DC;
    }
  }
  .chat-message-field__btn {
    display: block;
    width: 48px;
    height: 48px;
    outline: none;
    border: 0;
    border-radius: 50%;
    background: linear-gradient(to right, #009eb7 0%, #80deea 100%);
    overflow: hidden;
    &:hover {
      background: #009EB7;
    }
    &:active {
      background: #009EB7;
    }
  }
  .chat-message-field__btn-icon {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 18px;
    height: 13px;
    fill: #fff;
  }
</style>
