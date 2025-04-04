<template>
  <view class="p-2 bg-gray-50">
    <wd-button type="success">成功按钮</wd-button>
    <wd-button type="info">信息按钮</wd-button>

    <wd-cell title="手机号" :arrow="false" required>
      <button class="open-button" size="mini" open-type="getPhoneNumber">
         未设置
        <wd-icon name="arrow-right" color="#909399" class="ml-2"></wd-icon>
      </button>
    </wd-cell>

    <wd-cell-group custom-class="mt-10" border>
      <wd-cell title="标题文字" value="内容"/>
      <wd-cell title="标题文字" label="描述信息" value="内容"/>
    </wd-cell-group>

    <wd-card title="经营分析" custom-class="!mt-10" border>
      一般的，经营分析经营分析经营分析经营分析经营分析经营分析经营分析经营分析经营分析经营分析经营分析经营分析。
      <template #footer>
        <wd-button size="small" plain>查看详情</wd-button>
      </template>
    </wd-card>
  </view>
</template>

<script setup lang="ts">
</script>

<style scoped lang="scss">

//1、当存在复合选择器或是伪类时，会导致其它框架的css失效，貌似是影响var()相关变量
//2、而且热加载无效，要想查看效果必须重新运行`npm run dev:mp-weixin`
//3、甚至下方即便注释也会影响，只有删除下方代码才正常或不同复合选择器、伪类时正常
//复合选择器
/*button.open-button {
  background: #fff;
  padding: 0;
  color: #57595c;
}*/
//伪类
/*.open-button::after {
  border: none;
}*/
</style>
