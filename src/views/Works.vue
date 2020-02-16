<template>
  <div class="works">
    <h1 class="title">Works</h1>
    <div>
      <ul class="works_list">
        <li v-for="work in works" v-bind:key="work" class="work">
          <div class="work-thumbnail">
            <img v-bind:src="work.thumbnail" alt />
          </div>
          <div class="work-data">
            <h2 class="work-title">{{ work.title }}</h2>
            <div class="work-body">{{ work.body }}</div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "works",
  data() {
    return {
      works: [
        {
          thumbnail: "//placehold.jp/128x128.png",
          title: "ここに案件名Aがはいります",
          body:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium consequuntur animi dolore ipsum pariatur asperiores sit suscipit temporibus iusto quaerat numquam, enim voluptas. Magnam omnis, nam sunt maiores quae eaque. Lorem ipsum dolor sit, amet consectetur adipisicing elit. Soluta, eveniet! Lorem ipsum dolor sit, amet consectetur adipisicing elit. Soluta, eveniet!"
        },
        {
          thumbnail: "//placehold.jp/128x128.png",
          title: "ここに案件名Bがはいります",
          body:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo blanditiis illum saepe aliquid."
        },
        {
          thumbnail: "//placehold.jp/128x128.png",
          title: "ここに案件名Cがはいります",
          body:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Expedita laborum tenetur maiores voluptatibus alias optio, sunt distinctio harum ipsa quibusdam dolores consequuntur ipsum reiciendis dolor nisi ullam iusto!"
        },
        {
          thumbnail: "//placehold.jp/128x128.png",
          title: "ここに案件名Dがはいります",
          body:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eaque, explicabo!"
        },
        {
          thumbnail: "//placehold.jp/128x128.png",
          title: "ここに案件名Eがはいります",
          body: "Lorem ipsum, dolor sit amet consectetur adipisicing elit."
        },
        {
          thumbnail: "//placehold.jp/128x128.png",
          title: "ここに案件名Fがはいります",
          body:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium consequuntur animi dolore ipsum pariatur asperiores sit suscipit temporibus iusto quaerat numquam, enim voluptas. Magnam omnis, nam sunt maiores quae eaque. Lorem ipsum dolor sit, amet consectetur adipisicing elit. Soluta, eveniet! Lorem ipsum dolor sit."
        },
        {
          thumbnail: "//placehold.jp/128x128.png",
          title: "ここに案件名Gがはいります",
          body:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi, reiciendis. Totam ipsam tempora, sit dolorum aut natus pariatur."
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.works {
}
.works_list {
}
.work {
  flex: 0 0 auto;
  display: flex;
  flex-wrap: wrap;
  padding: 16px 16px 24px;
  margin-bottom: 1rem;
  background-color: #fff;
  text-shadow: none;
  text-align: left;
  border-radius: 4px;
  box-shadow: 0px 2px 8px rgba(66, 42, 42, 0.16);
  &-thumbnail {
    flex: 0 0 128px;
    margin-right: 16px;
    img {
      border-radius: 8px;
    }
  }
  &-data {
    flex: 1 0 auto;
    color: #111;
    word-break: break-all;
    overflow-wrap: break-word;
    max-width: calc(100% - 160px);
  }
  &-title {
    margin-bottom: 0.25rem;
    font-size: 1.25rem;
    font-weight: bold;
    color: #222;
  }
}
@media screen and (min-width: 768px) {
  .works_list {
    display: flex;
    margin: auto;
    max-width: 100%;
    flex-wrap: wrap;
  }
  .work {
    flex: 0 0 calc(50% - 0.5rem);
    &:nth-child(even) {
      margin-left: 1rem;
    }
  }
}
@media screen and (min-width: 1280px) {
  .work {
    flex: 0 0 calc(25% - 0.75rem);
    margin-left: 1rem;
    display: block;
    &:nth-child(4n + 1) {
      margin-left: 0px;
    }
    &-thumbnail {
      margin-right: 0;
      text-align: center;
    }
    &-data {
      max-width: 100%;
    }
    &-title {
      margin-bottom: 0.25rem;
      font-size: 1.25rem;
      font-weight: bold;
    }
  }
}
</style>
