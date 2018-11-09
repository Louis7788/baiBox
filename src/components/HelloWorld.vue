  <template>
    <div class="panel">
  <el-tabs v-model="activeName"  type="border-card" @tab-click="handleClick">
    <el-tab-pane label="图片" name="first">
    <el-card class="box-card" v-for="o in 10" :key="o">
  <div v-for="o in 4" :key="o" class="text item">
    {{'列表内容 ' + o }}
  </div>
</el-card>
    </el-tab-pane>
    <el-tab-pane label="二维码" name="second">  <el-card class="box-card" v-for="o in 10" :key="o">
  <div v-for="o in 4" :key="o" class="text item">
    {{'列表内容 ' + o }}
  </div>
</el-card></el-tab-pane>
    <el-tab-pane label="视频" name="third">  <el-card class="box-card" v-for="o in 10" :key="o">
  <div v-for="o in 4" :key="o" class="text item">
    {{'列表内容 ' + o }}
  </div>
</el-card></el-tab-pane>
    <el-tab-pane label="日常生活" name="fourth">  <el-card class="box-card" v-for="o in 10" :key="o">
  <div v-for="o in 4" :key="o" class="text item">
    {{'列表内容 ' + o }}
  </div>
</el-card></el-tab-pane>
     <el-tab-pane label="高效工作" name="first1">  <el-card class="box-card" v-for="o in 10" :key="o">
  <div v-for="o in 4" :key="o" class="text item">
    {{'列表内容 ' + o }}
  </div>
</el-card></el-tab-pane>
    <el-tab-pane label="电商" name="second1">  <el-card class="box-card" v-for="o in 10" :key="o">
  <div v-for="o in 4" :key="o" class="text item">
    {{'列表内容 ' + o }}
  </div>
</el-card></el-tab-pane>
    <el-tab-pane label="程序员" name="third1">  <el-card class="box-card" v-for="o in 10" :key="o">
  <div v-for="o in 4" :key="o" class="text item">
    {{'列表内容 ' + o }}
  </div>
</el-card></el-tab-pane>
    <el-tab-pane label="微信公众号" name="fourt1h">  <el-card class="box-card" v-for="o in 10" :key="o">
  <div v-for="o in 4" :key="o" class="text item">
    {{'列表内容 ' + o }}
  </div>
</el-card></el-tab-pane>
  </el-tabs>
    </div>
  </template>
  <script>
export default {
  name: "HelloWorld",
  data() {
    return {
      activeName: "second"
    };
  },
  methods: {
    handleClick(tab, event) {
      console.log(tab, event);
    }
  }
};
</script>

  <style scoped>
.panel {
  margin-left: 200px;
}
.box-card {
  width: 20%;
  margin-bottom: 10px;
  margin-right: 10px;
  display: inline-block;
  float: left;
}
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
