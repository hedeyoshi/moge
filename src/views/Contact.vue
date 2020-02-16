<template>
  <div class="contact">
    <h1 class="title">Contact</h1>
    <p>お問い合わせはこちらから</p>
    <a href="mailto:user@dammy.com" class="mail">
      <img src="../assets/mail_outline-24px.svg" alt="mail" />
    </a>
  </div>
</template>

<script>
export default {
  name: 'contact',
};
</script>

<style lang="scss" scoped>
.contact {
}
.mail {
  display: inline-block;
  padding: 16px;
  margin: 1rem;
  background: #fff;
  border-radius: 32px;
  transition: ease 0.3s;
  &:hover,
  &:focus {
    background-color: #deff22;
  }
  img {
    display: inline-block;
    vertical-align: bottom;
  }
}
</style>
