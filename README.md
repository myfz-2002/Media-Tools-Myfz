<!-- Media Tools - README.html 样式（可直接用于 GitHub README.md） -->
<div align="center">
  <h1>Media Tools</h1>
  <p>Android 本地 & 远程音视频播放工具</p>
</div>
### 📊 项目信息
![GitHub stars](https://img.shields.io/github/stars/myfz-2002/MediaTools?style=flat&label=Stars&color=yellow)
![GitHub forks](https://img.shields.io/github/forks/myfz-2002/MediaTools?style=flat&label=Forks&color=blue)
![GitHub contributors](https://img.shields.io/github/contributors/myfz-2002/MediaTools?style=flat&label=Contributors&color=green)
![GitHub last commit](https://img.shields.io/github/last-commit/myfz-2002/MediaTools?style=flat&label=Last%20Commit&color=orange)
![GitHub repo size](https://img.shields.io/github/repo-size/myfz-2002/MediaTools?style=flat&label=Repo%20Size&color=purple)
![GitHub downloads](https://img.shields.io/github/downloads/myfz-2002/MediaTools/total?style=flat&label=Downloads&color=red)
![GitHub license](https://img.shields.io/github/license/myfz-2002/MediaTools?style=flat&label=License&color=green)

---

 
<h2>1. 开发环境</h2>
<ul>
  <li>AIDE+ (AIDE Plus)</li>
  <li>Android SDK 5.0+ (API 21+)</li>
  <li>Gradle 4.6+</li>
  <li>Java 8</li>
</ul>

<h2>2. 模块划分</h2>
<table>
  <thead>
    <tr>
      <th>模块</th>
      <th>简要说明</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>播放核心服务</td>
      <td>音视频播放管理、后台播放、音频焦点、状态监听</td>
    </tr>
    <tr>
      <td>本地文件浏览</td>
      <td>扫描本地音频/视频、展示文件信息、分类管理</td>
    </tr>
    <tr>
      <td>远程连接播放</td>
      <td>支持网络地址、局域网、流媒体链接播放</td>
    </tr>
    <tr>
      <td>主界面</td>
      <td>媒体分类、最近播放、收藏、播放列表入口</td>
    </tr>
    <tr>
      <td>播放器界面</td>
      <td>进度控制、播放模式、封面、时长、播放列表操作</td>
    </tr>
  </tbody>
</table>

<h2>3. 实现功能</h2>
<ol>
  <li>扫描并展示本地音频、视频文件</li>
  <li>播放、暂停、上一曲、下一曲、进度拖动</li>
  <li>支持远程网络链接播放（http/https）</li>
  <li>播放列表记忆，重启自动恢复</li>
  <li>顺序播放、单曲循环、随机播放</li>
  <li>后台播放 + 通知栏控制</li>
  <li>音频焦点管理，被打断后自动恢复</li>
  <li>封面加载、时长显示、文件信息展示</li>
  <li>收藏、播放列表增删改查</li>
  <li>简洁 UI，适配手机与平板</li>
</ol>

<h2>4. 依赖库（代码框）</h2>
<pre>
// 音视频播放
implementation 'com.google.android.exoplayer:exoplayer-core:2.19.1'
implementation 'com.google.android.exoplayer:exoplayer-ui:2.19.1'

// 网络请求
implementation 'com.squareup.okhttp3:okhttp:4.10.0'

// 图片加载
implementation 'com.github.bumptech.glide:glide:4.15.1'
annotationProcessor 'com.github.bumptech.glide:compiler:4.15.1'

// 数据库
implementation 'org.litepal.android:core:3.2.3'
</pre>

<h2>5. 目录结构说明</h2>
<h3>Java 文件</h3>
<table>
  <tr><th>路径</th><th>作用</th></tr>
  <tr><td>service/</td><td>播放服务、后台管理</td></tr>
  <tr><td>ui/activity/</td><td>页面 Activity</td></tr>
  <tr><td>ui/adapter/</td><td>列表适配器</td></tr>
  <tr><td>bean/</td><td>媒体实体类</td></tr>
  <tr><td>engine/</td><td>播放引擎、ExoPlayer 管理</td></tr>
  <tr><td>utils/</td><td>工具类</td></tr>
  <tr><td>db/</td><td>数据库（收藏、历史）</td></tr>
</table>

<h3>XML 资源</h3>
<table>
  <tr><th>路径</th><th>作用</th></tr>
  <tr><td>layout/activity_*.xml</td><td>界面布局</td></tr>
  <tr><td>layout/item_*.xml</td><td>列表项布局</td></tr>
  <tr><td>drawable/</td><td>图标、样式、背景</td></tr>
  <tr><td>values/colors.xml</td><td>颜色配置</td></tr>
  <tr><td>values/styles.xml</td><td>主题样式</td></tr>
</table>

<h2>💖 鸣谢</h2>
<p>本项目使用以下优秀开源库，特此致谢：</p>
<ul>
  <li><strong>ExoPlayer</strong> - Google 官方音视频播放引擎</li>
  <li><strong>Glide</strong> - 高效图片加载库</li>
  <li><strong>OkHttp</strong> - 网络请求框架</li>
  <li><strong>LitePal</strong> - 轻量级 ORM 数据库</li>
</ul>

<div align="center" style="margin-top:30px;">
  <p>Media Tools © 2026 | 本地 + 远程音视频播放器</p>
</div>
