# Media Tools
Android 本地 & 远程音视频播放工具


## 📊 项目信息
![Stars](https://img.shields.io/github/stars/myfz-2002/MediaTools?style=flat-square&label=Stars&color=yellow)
![Forks](https://img.shields.io/github/forks/myfz-2002/MediaTools?style=flat-square&label=Forks&color=blue)
![Contributors](https://img.shields.io/github/contributors/myfz-2002/MediaTools?style=flat-square&label=Contributors&color=green)
![Last Commit](https://img.shields.io/github/last-commit/myfz-2002/MediaTools?style=flat-square&label=Last%20Commit&color=orange)
![Repo Size](https://img.shields.io/github/repo-size/myfz-2002/MediaTools?style=flat-square&label=Repo%20Size&color=purple)
![License](https://img.shields.io/github/license/myfz-2002/MediaTools?style=flat-square&label=License&color=green)
## 1. 开发环境
- AIDE+ (AIDE Plus)
- Android SDK 5.0+ (API 21+)
- Gradle 8.5
- Java 8
## 2. 模块划分
| 模块 | 简要说明 |
| --- | --- |
| 播放核心服务 | 音视频播放管理、后台播放、音频焦点、状态监听 |
| 本地文件浏览 | 扫描本地音频/视频、展示文件信息、分类管理 |
| 远程连接播放 | 支持网络地址、局域网、流媒体链接播放 |
| 主界面 | 媒体分类、最近播放、收藏、播放列表入口 |
| 播放器界面 | 进度控制、播放模式、封面、时长、播放列表操作 |
## 3. 实现功能
1. 扫描并展示本地音频、视频文件
2. 播放、暂停、上一曲、下一曲、进度拖动
3. 支持远程网络链接播放（http/https）
4. 顺序播放、单曲循环、随机播放
5. 后台播放 + 通知栏控制
6. 音频焦点管理，被打断后自动恢复
7. 封面加载、时长显示、文件信息展示
8. 收藏、播放列表增删改查
## 4. 依赖库
```gradle
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

### 模块6：开源依赖&许可证
```markdown
## 💖 开源依赖 & 许可证
本项目基于以下优秀开源项目开发，感谢所有贡献者：

- **IJKPlayer**  
  许可证：GPL-2.0 / GPL-3.0 / LGPL-3.0  
  项目地址：[https://github.com/Bilibili/ijkplayer](https://github.com/Bilibili/ijkplayer)

- **VideoCache（视频缓存）**  
  许可证：Apache License 2.0  
  项目地址：[https://github.com/danikula/AndroidVideoCache](https://github.com/danikula/AndroidVideoCache)

- **Glide（滑行）**  
  许可证：Apache License 2.0  
  项目地址：[https://github.com/bumptech/glide](https://github.com/bumptech/glide)

- **ExoPlayer**  
  许可证：Apache License 2.0  
  项目地址：[https://github.com/google/ExoPlayer](https://github.com/google/ExoPlayer)

- **CircleImageView（圆形图像视图）**  
  许可证：Apache License 2.0  
  项目地址：[https://github.com/hdodenhof/CircleImageView](https://github.com/hdodenhof/CircleImageView)

- **StatusBarUtil（状态栏实用程序）**  
  许可证：Apache License 2.0  
  项目地址：[https://github.com/laobie/StatusBarUtil](https://github.com/laobie/StatusBarUtil)

- **OkHttp**  
  许可证：Apache License 2.0  
  项目地址：[https://github.com/square/okhttp](https://github.com/square/okhttp)

- **LitePal（光之伙伴）**  
  许可证：Apache License 2.0  
  项目地址：[https://github.com/LitePalFramework/LitePal](https://github.com/LitePalFramework/LitePal)

- **JiaoZiVideoPlayer（娇子视频播放器）**  
  许可证：MIT License  
  项目地址：[https://github.com/lipangit/JiaoZiVideoPlayer](https://github.com/lipangit/JiaoZiVideoPlayer)

- **SimpleMusic（简易音乐）**  
  许可证：GPL-3.0  
  项目地址：[https://github.com/ikunjee/SimpleMusic](https://github.com/ikunjee/SimpleMusic)

---
<div align="center">
  <p>Media Tools © 2026 | 本地 + 远程音视频播放器</p>
  <p>部分代码使用AI辅助编写</p>
</div>
