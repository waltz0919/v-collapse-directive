# v-collapse
vue自定义收放指令



##### 使用方法：

#### template：v-collapse绑定在父容器上，子元素高度设为100%。

参数值：{ open：容器展开时的高度（string），close：容器收起时的高度（string），icon：按钮图标类名，style：按钮样式 }

```vue
 <div v-collapse="{open:'200px',close:'43px'}"> 
   <el-table :data="[{ date: '2016-05-02', name: '王小虎', address: '上海市普陀区金沙江路 1518 弄' }, { date: '2016-05-04', name: '王小虎', address: '上海市普陀区金沙江路 1517 弄' }]" style="width: 100%;height:100%;"> 
    <el-table-column prop="date" label="日期" width="180" /> 
    <el-table-column prop="name" label="姓名" width="180" /> 
    <el-table-column prop="address" label="地址" /> 
   </el-table> 
  </div>
```

#### main：

```js
import collapse from 'collapse'
Vue.use(collapse)
```

