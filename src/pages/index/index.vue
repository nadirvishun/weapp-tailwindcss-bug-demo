<template>
  <view class="p-2 bg-gray-50">
    <wd-button type="success">成功按钮</wd-button>
    <wd-button type="info">信息按钮</wd-button>

    <wd-cell-group custom-class="mt-10" border>
      <wd-cell title="标题文字" value="内容" />
      <wd-cell title="标题文字" label="描述信息" value="内容" />
    </wd-cell-group>

    <wd-cell-group custom-class="mt-10" border>
      <wd-cell icon="setting1" title="称重设置" clickable is-link></wd-cell>
      <wd-cell icon="money-circle" title="会员记录" clickable is-link></wd-cell>
      <wd-cell icon="help-circle" title="使用帮助" clickable is-link></wd-cell>
    </wd-cell-group>

    <wd-card title="经营分析" custom-class="mt-10!" >
      一般的，检举内容由承办的党的委员会或纪律检查委员会将处理意见或复议、复查结论同申诉人见面，听取其意见。复议、复查的结论和决定，应交给申诉人一份。
      <template #footer>
        <wd-button size="small" plain>查看详情</wd-button>
      </template>
    </wd-card>
  </view>
</template>

<script setup lang="ts">
import { ref } from 'vue'
const title = ref('Hello')
</script>

<style>

</style>
