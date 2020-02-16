<template>
  <ul>
    <li class="work">
      <img src="//placehold.jp/150x150.png" alt="" class="work-thumbnail" />
      <h2 class="work-title">案件名</h2>
      <div class="work-data">
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium
          consequuntur animi dolore ipsum pariatur asperiores sit suscipit
          temporibus iusto quaerat numquam, enim voluptas. Magnam omnis, nam
          sunt maiores quae eaque.
        </p>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Soluta,
          eveniet!
        </p>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Soluta,
          eveniet!
        </p>
      </div>
    </li>
  </ul>
</template>

<script>
export default {
  name: 'Work',
  props: {
    logo: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.Navigation {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  box-shadow: 0 0 32px 0 rgba(0, 0, 0, 0.16);
  font-family: 'Roboto', sans-serif;
  ul {
    display: flex;
    justify-content: center;
    align-items: stretch;
  }
  li {
    flex: 1 0 auto;
  }
  a {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 48px;
    background-color: #fff;
    text-decoration: none;
    transition: ease 0.16s;
    &:link,
    &:visited {
      color: #111111;
    }
    &:active {
    }
    &:hover,
    &:focus {
      color: #ff1940;
    }
  }
  .router-link-active {
    background-color: #deff22;
  }
}
</style>
