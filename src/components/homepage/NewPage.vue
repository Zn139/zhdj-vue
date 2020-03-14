<template>
    <div>
      <Header></Header>
      <div class="word">
        <div class="bodier">
        	<div class="titlename" label="11111"><span >新闻资讯</span></div>
        	<ul>
            <Item v-for="(article,index) in articles" :key="index" :article="article"></Item>
        	</ul>
        </div>
      </div>
    </div>
</template>

<script>
  import Item from './Item.vue'
  import Header from '@/components/common/Header'
  export default {
    name: "NewPage",
    /*
    data () {
        return {
          articles: []// 开始页面为空
        }
      },
      created () {
        this.$http.get('articles').then(res => {
          //this.articles = res.data
          this.articles.unshift(res.data)

          //  import axios from 'axios'
           // Vue.prototype.$http = axios.create({// 创建一个请求实例
           //   baseURL: 'http://localhost:3001/api'
           // })// 定义一个接口和地址，效果：在任意页面上使用this.$http访问axios实例
            // Vue.config.productionTip = false// 消息提示的环境配置，设置为开发环境或者生产环境


        })
      }
    };
    */
    data () {
      return {
        articles: [
          {
            //aUrl
            //imgUrl
            // 居然会跳转
            title: '较真碰硬“督” 凝心聚力“战”——习近平总书记在决战决胜脱贫攻坚座谈会上重要讲话引发强烈反响',
            time: '10小时前',// ?
            author: '朱雪梅',
            province: '河北省',
            common_num: 0,// 前台计算还是后台计算
            new: 'news'
          },
          {
            title: '较真碰硬“督” 凝心聚力“战”——习近平总书记在决战决胜脱贫攻坚座谈会上重要讲话引发强烈反响',
            time: '10小时前',
            author: '朱雪梅',
            province: '河北省',
            common_num: 0,
            new: 'news'
          },
          {
            title: '较真碰硬“督” 凝心聚力“战”——习近平总书记在决战决胜脱贫攻坚座谈会上重要讲话引发强烈反响',
            time: '10小时前',
            author: '朱雪梅',
            province: '河北省',
            common_num: 0,
            new: 'news'
          },
          {
            title: '较真碰硬“督” 凝心聚力“战”——习近平总书记在决战决胜脱贫攻坚座谈会上重要讲话引发强烈反响',
            time: '10小时前',
            author: '朱雪梅',
            province: '河北省',
            common_num: 0,
            new: 'news'
          },
          {
            title: '较真碰硬“督” 凝心聚力“战”——习近平总书记在决战决胜脱贫攻坚座谈会上重要讲话引发强烈反响',
            time: '10小时前',
            author: '朱雪梅',
            province: '河北省',
            common_num: 0,
            new: 'news'
          },
          {
            title: '较真碰硬“督” 凝心聚力“战”——习近平总书记在决战决胜脱贫攻坚座谈会上重要讲话引发强烈反响',
            time: '10小时前',
            author: '朱雪梅',
            province: '河北省',
            common_num: 0,
            new: 'news'
          },
          {
            title: '较真碰硬“督” 凝心聚力“战”——习近平总书记在决战决胜脱贫攻坚座谈会上重要讲话引发强烈反响',
            time: '10小时前',
            author: '朱雪梅',
            province: '河北省',
            common_num: 0,
            new: 'news'
          },
          {
            title: '较真碰硬“督” 凝心聚力“战”——习近平总书记在决战决胜脱贫攻坚座谈会上重要讲话引发强烈反响',
            time: '10小时前',
            author: '朱雪梅',
            province: '河北省',
            common_num: 0,
            new: 'news'
          },
          {
            title: '较真碰硬“督” 凝心聚力“战”——习近平总书记在决战决胜脱贫攻坚座谈会上重要讲话引发强烈反响',
            time: '10小时前',
            author: '朱雪梅',
            province: '河北省',
            common_num: 0,
            new: 'news'
          }
        ]
      }
    },
    components: {
      Header,
      Item
    }
  }
</script>

<style scoped>
 /* .word {
    font-size: 20px;
    font-weight: bolder;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }*/
  .bodier{
  	padding-top: 50px;
  	padding-left: 90px;
  	background-color: #F2F2F2;/*qq截图时ctrl+C可以复制色号*/
  }
  /*新闻资讯*/
  .titlename{
  	width: 1170px;
  	height: 20px;
  	padding: 16px;
  	background-color: white;
    font-size: 14px;
  }
  ul li{
  	width: 1170px;
  	height:44px ;
  	list-style: none;/*去掉列表前面的点*/
  	padding: 16px;
  	margin: 0;
  	border-top: dotted 1px #CCCCCC;/*dotted点线、dashed虚线、solid实线、double双线、inset 3D嵌入式边框、outset 3D突出式边框*/
  	/*border-color: #0000FF; 设置3D时要设置边框颜色，但效果依旧不明显*/
  	text-align: top;
  	background-color: white;
  	display: block;/*将该行内元素变为框*/
  }

</style>
