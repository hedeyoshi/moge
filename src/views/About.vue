<template>
  <div class="about">
    <h1 class="title">About</h1>
    <img src="../assets/icon.png" alt="icon" class="icon" /><br />
    <dl>
      <dt>Name</dt>
      <dd>Hideyoshi Koeda</dd>
      <dt>Skill</dt>
      <dd>
        html5, css3, jQuery, javascript, illustration
      </dd>
      <dt>Tool</dt>
      <dd>
        VSCode, Adobe XD, Photoshop, SAI2
      </dd>
    </dl>
  </div>
</template>

<script>
export default {
  name: 'about',
};
</script>

<style lang="scss" scoped>
.about {
  dl {
    margin-top: 1rem;
  }
  dt {
    font-weight: bold;
    font-size: 1.2rem;
  }
  dd {
    margin-bottom: 1rem;
  }
}
</style>
