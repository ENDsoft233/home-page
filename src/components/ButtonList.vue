<template>
  <div class="button-list">
    <div class="container">
      <ul>
        <li><a rel="noopener" target="_blank" href="https://space.bilibili.com/24553739"><img src="https://pro-video.xiaoheiban.cn/qpn/cea1a68a-1095-411a-ba18-7977ac7b6a47.svg" alt="BiliBili" title="BiliBili"></a></li>
        <li><a rel="noopener" target="_blank" href="https://github.com/ENDsoft233"><img src="https://pro-video.xiaoheiban.cn/iod/c719a4dc-8343-4cd9-bf64-04d8ff64605b.svg" alt="Github" title="Github"></a></li>
        <!-- <li><a rel="noopener" target="_blank" href="https://user.qzone.qq.com/2549279658"><img src="https://pro-video.xiaoheiban.cn/mlz/4bb640ef-afac-4c03-bc8a-fec6bf2fbbba.svg" alt="Qzone" title="Qzone"></a></li> -->
        <li><a rel="noopener" target="_blank" href="https://SteamCommunity.com/id/ENDsoft233"><img src="https://pro-video.xiaoheiban.cn/veh/f09af134-d8f2-4ecd-82a6-6924db78c8fb.svg" alt="Steam" title="Steam"></a></li>
        <li><a rel="noopener" target="_blank" href="https://twitter.com/ENDsoft233"><img src="https://pro-video.xiaoheiban.cn/tdj/08a5fb5a-dc48-4012-b9f7-2cebc1b185e6.svg" alt="Twitter" title="Twitter"></a></li>
        <li><a rel="noopener" target="_blank" href="https://zhihu.com/people/dtraywong"><img src="https://pro-video.xiaoheiban.cn/hgj/981bafc6-98d5-48c9-877c-b47779aa0dd3.svg" alt="知乎" title="知乎"></a></li>
        <!-- <li><a rel="noopener" target="_blank" href="https://weibo.com/ENDsoft"><img src="https://pro-video.xiaoheiban.cn/pyp/e5ec5a45-7db3-4e10-9498-d305f95e09ff.svg" alt="Weibo" title="Weibo"></a></li> -->
        <li><a rel="noopener" target="_blank" href="mailto://i@r-ay.cn"><img src="https://pro-video.xiaoheiban.cn/pyp/5ecb7351-bb70-4f28-a577-a6c5eee0bb16.svg" alt="Email" title="Email"></a></li>
        <li><a rel="noopener" target="_blank" href="https://blog.r-ay.cn"><span title="博客">Blog</span></a></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ButtonList'
}
</script>

<style lang="sass" scoped>
@import "src/assets/style/global"
.button-list
  display: block
  min-width: 100%
  /*margin-top: 30px*/
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
    img
      width: 60%
      height: 60%
</style>
