<template>
  <div class="index">
    <div class="carousel">
        <el-carousel :interval="3000" type="card" height="200px" arrow="always">
          <el-carousel-item v-for="item in pictures" :key="item.id">
            <img style="width: 450px;height: 200px" :src="item.url"/>
          </el-carousel-item>
        </el-carousel>
    </div>
    <div class="banner">
      <img src="../../assets/img/home/banner.jpg"/>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'index',
    data() {
      return {
        pictures: [
          {id: 1, url: 'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1571916738734&di=1373491b20e81382987f5d5fc66cb4a2&imgtype=0&src=http%3A%2F%2Fpic19.nipic.com%2F20120307%2F8071875_105010507157_2.jpg'},
          {id: 2, url: 'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1571916738734&di=1373491b20e81382987f5d5fc66cb4a2&imgtype=0&src=http%3A%2F%2Fpic19.nipic.com%2F20120307%2F8071875_105010507157_2.jpg'},
          {id: 3, url: 'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1571916738734&di=1373491b20e81382987f5d5fc66cb4a2&imgtype=0&src=http%3A%2F%2Fpic19.nipic.com%2F20120307%2F8071875_105010507157_2.jpg'},
          {id: 4, url: 'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1571916738734&di=1373491b20e81382987f5d5fc66cb4a2&imgtype=0&src=http%3A%2F%2Fpic19.nipic.com%2F20120307%2F8071875_105010507157_2.jpg'},
          {id: 5, url: 'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1571916738734&di=1373491b20e81382987f5d5fc66cb4a2&imgtype=0&src=http%3A%2F%2Fpic19.nipic.com%2F20120307%2F8071875_105010507157_2.jpg'}
        ]
      }
    }
  }
</script>

<style>
  .index{
    width: 100%;
  }
  .carousel{
    width: 900px;
    margin: 10px auto;
  }
  .banner{
    text-align: center;
    position: absolute;
    bottom: 0;
    left: 50%;
    transform: translate(-50%, 0);
  }
</style>
