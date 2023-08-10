<template>

<div>
<nut-tabbar @tab-switch="tabSwitch1" :tabbar-list="tabList6" :bottom="true">

</nut-tabbar>
</div>
</template>

<script setup>
export default {
  data() {
    return {
      tabList6: [
        {
          tabTitle: '定位',
          curr: true,
          href:"http://nutui.jd.com/demo.html#/index",
          icon: "https://img14.360buyimg.com/imagetools/jfs/t1/118307/14/13356/6509/5f1f964eE49521709/01d7262779580eae.png",
          activeIcon: "https://img13.360buyimg.com/imagetools/jfs/t1/144737/16/3979/6780/5f1f964eE1ea6a85c/f0884d425c08f817.png"
        },
        {
          tabTitle: '收藏',
          curr: false,
          isDot:true,
          href:"http://nutui.jd.com/demo.html#/index",
          icon: "https://img12.360buyimg.com/imagetools/jfs/t1/121804/37/8253/8253/5f1f964cE49319b40/e1013b7ecccddb9d.png",
          activeIcon: "https://img14.360buyimg.com/imagetools/jfs/t1/147105/26/3919/8702/5f1f964cEa84ada31/49449b6837783b96.png"
        },
        {
          tabTitle: '任务',
          curr: false,
          num:9,
          href:"http://nutui.jd.com/demo.html#/index",
          icon: "https://img13.360buyimg.com/imagetools/jfs/t1/135718/27/5479/4044/5f1f964cE2a855efc/be6cf14f8508d995.png",
          activeIcon: "https://img11.360buyimg.com/imagetools/jfs/t1/134812/35/5525/4171/5f1f964cE87259d35/0c15597415912785.png"
        },
        {
          tabTitle: '我的',
          curr: false,
          num:100,
          href:"http://nutui.jd.com/demo.html#/index",
          icon: "https://img10.360buyimg.com/imagetools/jfs/t1/134791/32/5470/6758/5f1f964cEa5ffb2c4/a001fcc43aebd555.png",
          activeIcon: "https://img12.360buyimg.com/imagetools/jfs/t1/141460/22/3921/6967/5f1f964cE0f298049/1aa9437df6e5e747.png"
        }
      ]
    };
  },
  methods: {
    tabSwitch1: function(value, index) {
      console.log(value, index);
    }
  }
};

</script>