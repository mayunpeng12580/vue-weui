<template>
  <div class="home">
    <h1>Hello World</h1>

    <!-- 主题样式 -->
    <we-button type="primary">按钮</we-button>
    <we-button type="warning">按钮</we-button>
    <we-button type="default" disabled>按钮</we-button>

    <!-- 线框 -->
    <we-button type="primary" plain>按钮</we-button>
    <we-button type="warning" plain>按钮</we-button>
    <we-button type="default" plain>按钮</we-button>
    <we-button type="default" plain>按钮</we-button>

    <!-- 控制大小 -->
    <we-button type="primary" size="large">按钮</we-button>
    <we-button type="primary" size="defaule">按钮</we-button>
    <we-button type="primary" size="mini">按钮</we-button>

  </div>
</template>

<script>
// @ is an alias to /src
import WeButton from '../components/WeButton';

export default {
  name:"home",
  components:{
    WeButton
  }

}
</script>
