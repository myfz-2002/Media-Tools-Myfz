<!-- Media Tools - README.html 样式（可直接用于 GitHub README.md） -->
<div align="center">
  <h1>Media Tools</h1>
  <p>Android 本地 & 远程音视频播放工具</p>
</div>

<h3>📊 项目信息</h3>
<img src="https://img.shields.io/github/stars/myfz-2002/MediaTools?style=flat&label=Stars&color=yellow" alt="GitHub stars">
<img src="https://img.shields.io/github/forks/myfz-2002/MediaTools?style=flat&label=Forks&color=blue" alt="GitHub forks">
<img src="https://img.shields.io/github/contributors/myfz-2002/MediaTools?style=flat&label=Contributors&color=green" alt="GitHub contributors">
<img src="https://img.shields.io/github/last-commit/myfz-2002/MediaTools?style=flat&label=Last%20Commit&color=orange" alt="GitHub last commit">
<img src="https://img.shields.io/github/repo-size/myfz-2002/MediaTools?style=flat&label=Repo%20Size&color=purple" alt="GitHub repo size">
<img src="https://img.shields.io/github/downloads/myfz-2002/MediaTools/total?style=flat&label=Downloads&color=red" alt="GitHub downloads">
<img src="https://img.shields.io/github/license/myfz-2002/MediaTools?style=flat&label=License&color=green" alt="GitHub license">

<hr>

 
<h2>1. 开发环境</h2>
<ul>
  <li>AIDE+ (AIDE Plus)</li>
  <li>Android SDK 5.0+ (API 21+)</li>
  <li>Gradle 8.5</li>
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
  
  <li>顺序播放、单曲循环、随机播放</li>
  <li>后台播放 + 通知栏控制</li>
  <li>音频焦点管理，被打断后自动恢复</li>
  <li>封面加载、时长显示、文件信息展示</li>
  <li>收藏、播放列表增删改查</li>

</ol>

<h2>4. 依赖库</h2>
<pre>
implementation 'com.android.support:appcompat-v7:28.0.0'
implementation 'com.android.support:support-core-utils:28.0.0'

implementation 'tv.danmaku.ijk.media:ijkplayer-java:0.8.8'
implementation 'tv.danmaku.ijk.media:ijkplayer-arm64:0.8.8'

implementation 'com.android.support:recyclerview-v7:28.0.0'
implementation 'com.danikula:videocache:2.7.0'
implementation 'com.github.bumptech.glide:glide:4.7.1'
implementation 'com.google.android.exoplayer:exoplayer:2.9.1'
implementation 'com.android.support.constraint:constraint-layout:1.1.3'
implementation 'com.android.support:support-v4:28.0.0'

implementation 'com.android.support:design:28.0.0'
implementation 'de.hdodenhof:circleimageview:3.0.0'
implementation 'com.jaeger.statusbarutil:library:1.4.0'
implementation "com.squareup.okhttp3:okhttp:3.12.0"

implementation "com.android.support:support-media-compat:28.0.0"

implementation 'com.github.bumptech.glide:glide:4.9.0'
implementation 'com.github.bumptech.glide:compiler:4.9.0'
implementation 'org.litepal.android:core:2.0.0'

api project(':jiaozivideoplayer')
</pre>

<h2>💖 开源依赖 & 许可证</h2>
<p>本项目基于以下优秀开源项目开发，感谢所有贡献者：</p>

<!-- 卡片式布局，带链接和许可证标识 -->
<div style="display: grid; grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); gap: 16px; margin: 20px 0;">


  <!-- IJKPlayer -->
  <div style="border: 1px solid #eee; padding: 16px; border-radius: 8px; background: #f9f9f9;">
    <h4 style="margin: 0 0 8px 0;"><a href="https://github.com/Bilibili/ijkplayer" target="_blank" style="color: #0366d6;">IJKPlayer</a></h4>
    <p style="margin: 0; color: #666;">许可证：GPL-2.0 / GPL-3.0 / LGPL-3.0</p>
  </div>

  <!-- VideoCache -->
  <div style="border: 1px solid #eee; padding: 16px; border-radius: 8px; background: #f9f9f9;">
    <h4 style="margin: 0 0 8px 0;"><a href="https://github.com/danikula/AndroidVideoCache" target="_blank" style="color: #0366d6;">VideoCache</a></h4>
    <p style="margin: 0; color: #666;">许可证：Apache License 2.0</p>
  </div>

  <!-- Glide -->
  <div style="border: 1px solid #eee; padding: 16px; border-radius: 8px; background: #f9f9f9;">
    <h4 style="margin: 0 0 8px 0;"><a href="https://github.com/bumptech/glide" target="_blank" style="color: #0366d6;">Glide</a></h4>
    <p style="margin: 0; color: #666;">许可证：Apache License 2.0</p>
  </div>

  <!-- ExoPlayer -->
  <div style="border: 1px solid #eee; padding: 16px; border-radius: 8px; background: #f9f9f9;">
    <h4 style="margin: 0 0 8px 0;"><a href="https://github.com/google/ExoPlayer" target="_blank" style="color: #0366d6;">ExoPlayer</a></h4>
    <p style="margin: 0; color: #666;">许可证：Apache License 2.0</p>
  </div>

  <!-- CircleImageView -->
  <div style="border: 1px solid #eee; padding: 16px; border-radius: 8px; background: #f9f9f9;">
    <h4 style="margin: 0 0 8px 0;"><a href="https://github.com/hdodenhof/CircleImageView" target="_blank" style="color: #0366d6;">CircleImageView</a></h4>
    <p style="margin: 0; color: #666;">许可证：Apache License 2.0</p>
  </div>

  <!-- StatusBarUtil -->
  <div style="border: 1px solid #eee; padding: 16px; border-radius: 8px; background: #f9f9f9;">
    <h4 style="margin: 0 0 8px 0;"><a href="https://github.com/laobie/StatusBarUtil" target="_blank" style="color: #0366d6;">StatusBarUtil</a></h4>
    <p style="margin: 0; color: #666;">许可证：Apache License 2.0</p>
  </div>

  <!-- OkHttp -->
  <div style="border: 1px solid #eee; padding: 16px; border-radius: 8px; background: #f9f9f9;">
    <h4 style="margin: 0 0 8px 0;"><a href="https://github.com/square/okhttp" target="_blank" style="color: #0366d6;">OkHttp</a></h4>
    <p style="margin: 0; color: #666;">许可证：Apache License 2.0</p>
  </div>

  <!-- LitePal -->
  <div style="border: 1px solid #eee; padding: 16px; border-radius: 8px; background: #f9f9f9;">
    <h4 style="margin: 0 0 8px 0;"><a href="https://github.com/LitePalFramework/LitePal" target="_blank" style="color: #0366d6;">LitePal</a></h4>
    <p style="margin: 0; color: #666;">许可证：Apache License 2.0</p>
  </div>

  <!-- JiaoZiVideoPlayer -->
  <div style="border: 1px solid #eee; padding: 16px; border-radius: 8px; background: #f9f9f9;">
    <h4 style="margin: 0 0 8px 0;"><a href="https://github.com/lipangit/JiaoZiVideoPlayer" target="_blank" style="color: #0366d6;">JiaoZiVideoPlayer</a></h4>
    <p style="margin: 0; color: #666;">许可证：MIT License</p>
  </div>

  <!-- SimpleMusic -->
  <div style="border: 1px solid #eee; padding: 16px; border-radius: 8px; background: #f9f9f9;">
    <h4 style="margin: 0 0 8px 0;"><a href="https://github.com/ikunjee/SimpleMusic" target="_blank" style="color: #0366d6;">SimpleMusic</a></h4>
    <p style="margin: 0; color: #666;">许可证：GPL-3.0</p>
  </div>
</div>

<div align="center" style="margin-top:30px; color: #888;">
  <p>Media Tools © 2026 | 本地 + 远程音视频播放器</p>
  <p>部分代码使用AI</p>
</div>

