<template>
  <el-row class="footer" tag="footer" type="flex" justify="space-around" align="middle">
    <el-col class="footer__contact" tag="section" :xl="4" :lg="4" :md="12" :sm="24" :xs="24">
      <h2>联系我们</h2>
      <ul class="contact__list">
        <li class="iconfont icon-xinfeng">
          <el-tooltip effect="dark" content="发送邮件" placement="top-start">
            <a href="mailto:2639415619@qq.com
        ?subject=古典文学名著阅读意见反馈">意见反馈</a>
          </el-tooltip>
        </li>
        <li class="iconfont icon-qq">
          <el-tooltip effect="dark" content="打开QQ" placement="top-start">
            <a href="tencent://message/?Site=baidu.com&uin=2639415619&Menu=yes">2639415619</a>
          </el-tooltip>
        </li>
        <li class="iconfont icon-xinfeng">
          <el-popover placement="top-start" width="150" trigger="hover">
            <img
              style="width: 150px"
              src="https://blog-luo.oss-cn-beijing.aliyuncs.com/qrcode/mmqrcode1580471197905.png"
              alt="微信二维码"
            />
            <a href="javascript:void(0)" slot="reference">Danyouqf2017</a>
          </el-popover>
        </li>
      </ul>
    </el-col>
    <el-col class="footer__about" :xl="4" :lg="4" :md="12" :sm="24" :xs="24">
      <h2>关于</h2>
      <ul class="contact__list">
        <li>
          <el-tooltip effect="dark" content="暂未开通" placement="top-start">
            <el-link style="margin-left: 0" type="info">古典文学名著阅读使用手册</el-link>
          </el-tooltip>
        </li>
        <li>
          <a style="margin-left: 0" href="javascript:void(0)" slot="reference">
            © 2019
            <el-link
              style="margin-left: 0"
              href="https://luoxuhai.netlify.com/"
              target="_blank"
              type="info"
            >luoxuhai</el-link>. All Rights Reserved.
          </a>
        </li>
        <li>
          <el-tooltip effect="dark" content="ICP备案查询" placement="top-start">
            <el-link
              style="margin-left: 0"
              type="info"
              href="http://beian.miit.gov.cn"
              target="_blank"
            >津ICP备 18009092号-1</el-link>
          </el-tooltip>
        </li>
      </ul>
    </el-col>
    <el-col class="footer__generalize" :xl="8" :lg="8" :md="8" :sm="24" :xs="24">
      <h2>更多</h2>
      <ul class="generalize__list">
        <li>
          <h5>快用工具小程序</h5>
          <img
            style="width: 150px"
            src="https://static.fastools.cn/images/miniapp.jpg"
            alt="微信二维码"
          />
        </li>
        <li>
          <h5>快用工具公众号</h5>
          <img
            style="width: 150px"
            src="
https://static.fastools.cn/images/qrcode.jpg?x-oss-process=style/fade"
            alt="微信二维码"
          />
        </li>
        <li>
          <el-tooltip effect="dark" content="Darkce" placement="top-start">
            <el-link type="info" href="https://www.fastools.cn/" target="_blank">快用工具官网</el-link>
          </el-tooltip>
        </li>
      </ul>
    </el-col>
  </el-row>
</template>

<style lang="scss" scoped>
// @import '@/assets/styles/utils.less';
h2 {
  margin-bottom: 30px;
  font-size: 22px;
  color: #333;
}

.footer {
  min-height: 450px;
  padding: 50px;
  background-color: #f7fbfd;
  flex-wrap: wrap;
  .footer__contact {
    display: flex;
    flex-direction: column;
    min-height: 300px;
    .contact__list {
      display: flex;
      flex-direction: column;
      justify-content: space-around;
      li {
        display: flex;
        align-items: center;
        margin-top: 40px;
        &::before {
          font-size: 22px;
        }
        a {
          margin-left: 20px;
          text-decoration: none;
          font-size: 16px;
          color: #666;
        }
      }
    }
  }

  .footer__about {
    @extend .footer__contact;
  }

  .footer__generalize {
    display: flex;
    flex-direction: column;
    height: 300px;
    .generalize__list {
      display: flex;
      align-items: flex-end;
      justify-content: space-between;
      li:last-child {
        a {
          font-size: 16px;
          color: #666;
        }
      }
      h5 {
        margin-bottom: 20px;
        font-size: 14px;
        color: #666;
      }
    }
  }
}
</style>
