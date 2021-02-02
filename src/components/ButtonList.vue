<template>
  <div class="button-list">
    <div class="container">
      <ul>
        <li v-for="(value, index) in list" :key="index">
          <a rel="noopener" target="_blank" :href="value.link">
            <img v-if="value.img" :src="value.img" :alt="value.title" :title="value.title">
            <span :title="value.title" v-else>{{ value.text }}</span>
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ButtonList',
  data() {
    return {
      list: [
        {
          img: 'https://pro-video.xiaoheiban.cn/qpn/cea1a68a-1095-411a-ba18-7977ac7b6a47.svg',
          title: 'BiliBili',
          link: 'https://space.bilibili.com/24553739'
        },
        {
          img: 'https://pro-video.xiaoheiban.cn/iod/c719a4dc-8343-4cd9-bf64-04d8ff64605b.svg',
          title: 'GitHub',
          link: 'https://github.com/ENDsoft233'
        },
        {
          img: 'https://pro-video.xiaoheiban.cn/veh/f09af134-d8f2-4ecd-82a6-6924db78c8fb.svg',
          title: 'Steam',
          link: 'https://SteamCommunity.com/id/ENDsoft233'
        },
        {
          img: 'https://pro-video.xiaoheiban.cn/tdj/08a5fb5a-dc48-4012-b9f7-2cebc1b185e6.svg',
          title: 'Twitter',
          link: 'https://twitter.com/ENDsoft233'
        },
        {
          img: 'https://pro-video.xiaoheiban.cn/hgj/981bafc6-98d5-48c9-877c-b47779aa0dd3.svg',
          title: 'Zhihu',
          link: 'https://zhihu.com/people/dtraywong'
        },
        {
          img: 'https://pro-video.xiaoheiban.cn/pyp/5ecb7351-bb70-4f28-a577-a6c5eee0bb16.svg',
          title: 'Email',
          link: 'mailto://i@r-ay.cn'
        },
        {
          text: 'Blog',
          title: '博客',
          link: 'https://blog.r-ay.cn'
        }
      ]
    }
  }
}
</script>

<style lang="sass" scoped>
@import "src/assets/style/global"
.button-list
  display: block
  min-width: 100%
  margin-top: 30px
.container
  max-width: 800px
  margin: 0 auto
  ul
    padding: 0
    margin: 0
    @include flex-center
    list-style: none
    flex-wrap: wrap
  li
    $box-size: 60px
    background-color: white
    border-radius: 50%
    height: $box-size
    width: $box-size
    line-height: $box-size
    margin: 10px 20px
    @include flex-center
    box-shadow: 0 0 0 0 rgba(white,0)
    transition: box-shadow .15s linear
    &:hover, &:active
      box-shadow: 0 0 0 10px rgba(white,.3)
    a
      @include flex-center
      text-decoration: none
      width: 100%
      height: 100%
      -webkit-tap-highlight-color: rgba(255,0,0,0)
      @include default-a
    span
      width: 80%
      word-break: break-all
      line-height: 1rem
    img
      width: 60%
      height: 60%
</style>
