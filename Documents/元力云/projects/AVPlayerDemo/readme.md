## 阿里视频组件

阿里高级视频播放器的简单 UI 封装，实现边下、边放、边缓存（下过一次后不会再下）。


# SimpleAVPlayer

功能：

1. 播放、暂停、继续播放、重放
2. 播放进度显示
3. loading 显示


用法：

```
NSURL* url = [NSURL URLWithString:@"http://221.4.63.91:8081/schcommonweb/weedfs/rdownload/2@8a54d21abc"];//@"http://192.168.20.25:28085/schcommonweb/weedfs/rdownload/2@8a54d21abc"];//@"https://mvvideo5.meitudata.com/56ea0e90d6cb2653.mp4"];//
    
_simplePlayer = [[SimpleAVPlayer alloc]initWithFrame:_videoView.bounds];
    
[self.videoView addSubview:_simplePlayer];
    
_simplePlayer.url= url;

```