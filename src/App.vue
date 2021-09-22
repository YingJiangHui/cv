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
import Link from './components/Link.vue'


</script>

<template>
  <CvContainer>
    <Article>
      <BaseInfo/>
      <Section>
        <template v-slot:title>
          <SectionTitle>工作经历</SectionTitle>
          <SectionSubTitle>杭州新之科技有限公司（2020-10 - 至今）</SectionSubTitle>
          <Paragraph>公司方向主要以可再生资源交易相关，提供再生资源的回收、加工和销售，完善回收的资金、物流数据链。通过与银行等各政府部门深度合作实现大额支付。</Paragraph>
          <Paragraph>前端技术主要以React为主，期间参加相关产品的技术选型，前端工程化相关构建，功能开发，维护迭代等。</Paragraph>
        </template>
      </Section>
      <Section>
        <template v-slot:title>
          <SectionTitle>项目经历</SectionTitle>
        </template>
        <SectionSubTitle>
          再生资源交易平台
        </SectionSubTitle>
        <Paragraph>介绍：提供再生资源产品的大额交易，买卖家入驻与管理，个体工商户的待办理，以及交易过程涉及的商品、物流、支付、开票、权限分配等。</Paragraph>
        <Paragraph>负责：支付模块、商品模块、物流等模块、买卖家模块的开发迭代，系统的维护，以及前端监控系统的集成，单元测试保证代码质量。</Paragraph>
        <Paragraph>技术：React、TypeScript、umi、Ant Design</Paragraph>
        <SectionSubTitle>再生资源监管平台</SectionSubTitle>
        <Paragraph>介绍：再生资源监管平台对再生资源交易的全过程进行跟踪监控，以及对于入驻用户的管理和维护。实现对资源回收再利用的溯源追踪</Paragraph>
        <Paragraph>负责：集团管理、开票管理、订单管理、支付管理、买卖家管理，税务管理等模块的开发迭代，系统的维护。以及<HighLightText>集成前端监控</HighLightText>、ui库升级、<HighLightText>框架迁移</HighLightText></Paragraph>
        <Paragraph>技术：React、TypeScript、umi、Ant Design、Ant Design Pro、dva</Paragraph>
        <SectionSubTitle>音视频采集</SectionSubTitle>
        <Paragraph>介绍：用于确认用户对于办理某业务的意向</Paragraph>
        <Paragraph>负责：项目的完整开发。主要包含：技术选型，项目搭建，音视频录制功能、TTS语言播报功能、语音识别功能</Paragraph>
        <Paragraph>技术：<HighLightText>webRTC</HighLightText>、webWorker、webSocket、TypeScript、React的移动端多媒体H5应用</Paragraph>
      </Section>
      <Section :whenPrintBreakPage="true">
        <template v-slot:title>
          <SectionTitle>技能</SectionTitle>
          <Paragraph>熟悉页面制作技巧，能将设计稿完美还原</Paragraph>
          <Paragraph>熟练掌握<HighLightText>TypeScript</HighLightText>，包括：泛型、类型工具函数等，对其他的强类型语言也有所了解</Paragraph>
          <Paragraph>熟练掌握<HighLightText>React</HighLightText>及其周边相关技术，包括Redux、hook等，了解React渲染调度机制</Paragraph>
          <Paragraph>熟练掌握<HighLightText>Vue</HighLightText>全家桶，包括Vuex、VueRouter</Paragraph>
          <Paragraph>掌握<HighLightText>Webpack</HighLightText>配置，有插件开源经历</Paragraph>
          <Paragraph>熟悉<HighLightText>ES6</HighLightText>语法，包括Promise、析构赋值等</Paragraph>
          <Paragraph>对后端技术有一定的了解，包括Sql、RESTful API、JWT、Session、cookie等</Paragraph>
          <Paragraph>熟悉数据结构和基本算法</Paragraph>
        </template>
        </Section>
      <Section>
        <template v-slot:title>
          <SectionTitle >开源项目</SectionTitle>
          <SectionSubTitle :links="[{href:'https://github.com/YingJiangHui/neat-ui-react',text:'源码地址'},{href:'https://yingjianghui.github.io/neat-ui-react/',text:'预览地址'}]">neat ui（迭代中）</SectionSubTitle>
          <Paragraph>基于 React + TypeScript 的ui库</Paragraph>
          <Paragraph>主打简洁、干净的ui设计，包括：主题功能、树形组件、下拉更新组件、各种通用型组件等。</Paragraph>
          <Paragraph>该项目使用了circle ci进行<HighLightText>持续集成</HighLightText>、使用 jest 进行<HighLightText>单元测试</HighLightText>，测试覆盖率达到80%以上</Paragraph>
          <Paragraph>该项目让我对BDD测试驱动开发得到了一定的实践，以及各种组件实现的原理，设计模式，对源码阅读能力有了显著的提升</Paragraph>
          <SectionSubTitle :links="[{href:'https://github.com/YingJiangHui/books-management-system-server',text:'后端源码地址'},{href:'https://github.com/YingJiangHui/books-management-system-admin-ui',text:'前端源码地址'}]">图书管理系统（前后端）</SectionSubTitle>
          <Paragraph>后端：Node、Nestjs、Postgres Sql、TS、TypeORM</Paragraph>
          <Paragraph>前端：React、TS、ECharts</Paragraph>
          <Paragraph>涉及 <HighLightText>登录注册</HighLightText>、<HighLightText>权限\角色管理</HighLightText>、用户邮箱验证，图书管理，用户对图书的借阅、预约、遗失等功能</Paragraph>
        </template>
      </Section>
      <Section>
        <template v-slot:title>
          <SectionTitle>其他连接</SectionTitle>
        </template>
        <Paragraph>
          <Link href="https://github.com/YingJiangHui">我的GitHib</Link> - 过去一年有近1000提交
        </Paragraph>

        <Paragraph>
          <Link href="https://github.com/YingJiangHui">我的博客</Link> - 目前已经发布了近40篇技术文章
        </Paragraph>
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
h3,h2,h1,p,ul,li,ol{
  margin: 0;
  padding: 0;
}
p,ul,li,ol{
  color: #666;
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
