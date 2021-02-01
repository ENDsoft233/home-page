<template>
  <base-layout>
      <avatar />
      <div class="name"><img height="72px" src="https://pro-video.xiaoheiban.cn/hcn/c18fcec0-94d4-4cb9-8db8-3284c88b1f23.svg" style="filter: invert(100%);" /></div>
      <button-list />
  </base-layout>
</template>

<script>
import Avatar from '@/components/Avatar'
import ButtonList from '@/components/ButtonList'
import BaseLayout from '@/components/BaseLayout'
export default {
  name: 'Home',
  components: {
    Avatar,
    ButtonList,
    BaseLayout
  }
}
</script>

<style lang="sass" scoped>
@import "src/assets/style/global"
.name
  /*margin-top: 30px*/
  font-size: 2.5rem
  color: white
</style>
