<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import HelloWorld from './components/HelloWorld.vue'
import Section from './components/Section.vue'
import Article from './components/Article.vue'
import CvContainer from './components/CvContainer.vue'
import SectionTitle from './components/SectionTitle.vue'
import SectionSubTitle from './components/SectionSubTitle.vue'
import Paragraph from "./components/Paragraph.vue";
import BaseInfo from "./components/BaseInfo.vue";
import HighLightText from "./components/HighLightText.vue";



</script>

<template>
  <CvContainer>
    <Article>
      <BaseInfo/>
      <Section>
        <template v-slot:title>
          <SectionTitle>项目经历</SectionTitle>
        </template>
        <SectionSubTitle>
          再生资源交易平台
        </SectionSubTitle>
        <Paragraph>再生资源电商交易平台</Paragraph>
        <Paragraph>主要负责支付模块、商品模块、物流等模块、买卖家模块的开发迭代，系统整体的维护，以及前端监控系统的集成、ui库升级，对关键函数、自定义hook进行了单元测试。</Paragraph>
        <Paragraph>基于：React、TypeScript、umi、Ant Design、Ant Design Pro 的Web端前后端分离项目</Paragraph>
        <SectionSubTitle>再生资源监管平台</SectionSubTitle>
        <Paragraph>介绍...</Paragraph>
        <Paragraph>主要负责集团管理、开票管理、订单管理、支付管理、买卖家管理，税务管理等模块的开发迭代，系统整体的维护。以及<HighLightText>集成前端监控</HighLightText>、ui库升级、<HighLightText>框架升级</HighLightText>，对关键函数、自定义hook进行了单元测试。</Paragraph>
        <Paragraph>基于：React、TypeScript、umi、Ant Design、Ant Design Pro 的Web端前后端分离项目</Paragraph>
        <SectionSubTitle>自研双录视频</SectionSubTitle>
        <Paragraph>用于确认用户对于办理某业务的意向</Paragraph>
        <Paragraph>独立负责项目从0到落地，主要包含：技术选型，项目搭建，音视频录制功能、TTS语言播报功能（调第三方API）、语音识别（调第三方API）。</Paragraph>
        <Paragraph>基于web RTC、web worker、web socket、TypeScript、React的移动端H5应用</Paragraph>
      </Section>
      <Section>
        <template v-slot:title>
          <SectionTitle>技能</SectionTitle>
          <Paragraph>熟练掌握TypeScript，包括：泛型、类型工具函数等，对其他的强类型语言也有所了解</Paragraph>
          <Paragraph>熟练掌握React及其周边相关技术，包括Redux、hook等，了解React渲染调度机制</Paragraph>
          <Paragraph>熟练掌握Vue全家桶，包括Vuex、VueRouter</Paragraph>
          <Paragraph>掌握Webpack配置，能够从零配置一个脚手架，编写过插件并向社区开源</Paragraph>
          <Paragraph>熟悉ES6语法，包括Promise、析构赋值等</Paragraph>
          <Paragraph>对后端技术有一定的了解，包括Sql、RESTful API、JWT、Session、cookie等</Paragraph>
          <Paragraph>熟悉数据结构和基本算法</Paragraph>
        </template>
        </Section>
      <Section>
        <template v-slot:title>
          <SectionTitle >开源经历</SectionTitle>
          <SectionSubTitle :links="[{href:'www.baidu.com',text:'百度'}]">neat-ui（迭代中）</SectionSubTitle>
          <Paragraph>基于 React + TypeScript 的ui库</Paragraph>
          <Paragraph>主打简洁、干净的ui设计，主要包括：树形组件、下拉更新组件、动画组件、各种通用型组件等。</Paragraph>
          <Paragraph>该项目使用了circle ci进行持续集成、使用jest了进行单元测试，测试覆盖率达到90%以上</Paragraph>
          <Paragraph>该项目让我对BDD测试驱动开发得到了一定的实践，以及各种组件实现的原理，对源码阅读能力有了一定的提升</Paragraph>
          <SectionSubTitle :links="[{href:'www.baidu.com',text:'百度'}]">图书管理系统</SectionSubTitle>
          <Paragraph>技术栈：后端：node、nestjs、postgres Sql、TS、TypeORM； 前端：React、TS、umi、Ant Design</Paragraph>
          <Paragraph>对于图书借阅预约的管理，以及相关的数据统计。</Paragraph>
          <Paragraph>涉及 <HighLightText>登录注册</HighLightText>、<HighLightText>权限\角色管理</HighLightText>、用户邮箱验证，图书管理，用户对图书的借阅、预约、遗失等功能</Paragraph>
          <Paragraph>该项目让我对后端开发</Paragraph>
        </template>
      </Section>
      <Section>
        <template v-slot:title>
          <SectionTitle>工作经历</SectionTitle>
          <SectionSubTitle :links="[{href:'www.baidu.com',text:'百度'}]">neat-ui（迭代中）</SectionSubTitle>
        </template>
      </Section>
      <Section>
        <template v-slot:title>
          <SectionTitle>教育经历</SectionTitle>
        </template>
      </Section>
      <Section>
        <template v-slot:title>
          <SectionTitle>其他连接</SectionTitle>
        </template>
      </Section>
    </Article>
  </CvContainer>
</template>

<style>
p{
  margin: 0;
  padding: 0;
  line-height: 1.5;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
h3,h2,h1,p,ul,ol{
  margin: 0;
  padding: 0;
}
body{
  background: #eeeeee
}
html,body{
  height: 100%;
}
ul,ol{
  list-style: none;
}
</style>
