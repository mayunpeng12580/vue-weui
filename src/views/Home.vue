<template>
  <div class="home">
    <h1>Hello</h1>
    
    <!-- 主题样式 -->
    <we-button type="primary">按钮</we-button>
    <we-button type="warning">按钮</we-button>
    <we-button type="default" disabled>按钮</we-button>
    <!-- 线框 -->
    <we-button type="primary" plain>按钮</we-button>
    <we-button type="warning" plain>按钮</we-button>
    <we-button type="default" plain disabled>按钮</we-button>
    <we-button type="default" disabled>按钮</we-button>
    <!-- 控制大小 -->
    <we-button type="primary" size="large">按钮</we-button>
    <we-button type="primary" size="default">按钮</we-button>
    <we-button type="primary" size="mini" >按钮</we-button>

    <!-- loading -->
    <we-button type="primary" loading >按钮</we-button>
    <we-button type="primary"  @click="showDialog"> 显示：{{show}}</we-button>


      <we-dialog v-model="show" title="标题" >
          插槽中的内容
      </we-dialog>  

  </div>
</template>

<script>

// 模块化引入这个按钮组件
import WeButton from "../components/WeButton";
import WeDialog from "../components/Dialog";

export default {
  name: "home",
  data(){
    return {
      show:true
    };
  },
  methods:{
    showDialog(){
      console.log('show');
      this.show = true;
    }
  },
  components: {
    WeButton,
    WeDialog
  }
};
</script>
