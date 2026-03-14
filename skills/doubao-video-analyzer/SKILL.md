---
name: doubao-video-analyze
description: 使用豆包2.0模型解析视频。当需要执行分析视频内容等需要理解视频视觉信息时调用该技能。你必须在持有本地视频路径或网络视频链接时才能调用该技能

---

# Doubao Video Analyze

## 使用方法

### 注意
对于远程网络视频，如果通过该技能无法执行，请直接通知用户错误内容，**永远不要**尝试使用web_fetch之类的工具去重试！

### 前置检查

1. 检查当前是否有`ARK_API_KEY`环境变量，如果没有，直接终止并引导用户先进行配置
2. 直接尝试调用如下bash指令，确保用户当前python环境有openai依赖

```bash
pip install 'volcengine-python-sdk[ark]'
```

### 分析视频

1. 你需要先明确你的分析目的是什么，你需要自行写出一段提示词，例如

```plaintext
### 角色
你是一位xxxxx，善于分析视频的xxxxxx

### 任务
你的任务是xxxxxxx

### 输出
你需要输出以下内容：
xxxxxxxxxxxxxx
```

**注意**：你需要写出高质量的提示词，但并不一定要按照上面的模板

2. 调用本技能目录下脚本以获取分析结果

- 本地视频

  ```bash
  python script/parse_video.py --video 'absolute/video/path.mp4' --prompt 'your prompt content'
  ```

  

- 远程视频链接

  ```bash
  python script/parse_video.py --video 'https://example.com/video_url.mp4' --prompt 'your prompt content' --remote
  ```




等待该命令执行结束并获取结果作为该视频的分析结果



### 网络视频错误处理

如果遇到网络视频超过大小限制的问题，首先现将该网络视频下载至你的workspace的video目录下，然后再通过本地视频的方式调用