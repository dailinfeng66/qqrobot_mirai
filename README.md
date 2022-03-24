```text
 ██ ███████    ████████ ████████ ████     ████       ██████     ███████   ██████████
░██░██░░░░██  ██░░░░░░ ░██░░░░░ ░██░██   ██░██      ░█░░░░██   ██░░░░░██ ░░░░░██░░░ 
░██░██    ░██░██       ░██      ░██░░██ ██ ░██      ░█   ░██  ██     ░░██    ░██    
░██░██    ░██░█████████░███████ ░██ ░░███  ░██ █████░██████  ░██      ░██    ░██    
░██░██    ░██░░░░░░░░██░██░░░░  ░██  ░░█   ░██░░░░░ ░█░░░░ ██░██      ░██    ░██    
░██░██    ██        ░██░██      ░██   ░    ░██      ░█    ░██░░██     ██     ░██    
░██░███████   ████████ ░████████░██        ░██      ░███████  ░░███████      ░██    
░░ ░░░░░░░   ░░░░░░░░  ░░░░░░░░ ░░         ░░       ░░░░░░░    ░░░░░░░       ░░     

```
## 基于Java Mirai的QQ机器人
### 主要功能
+ 进出校园打卡
+ 九价疫苗秒杀提醒


### 开发
#### 思想
     一个插件对应的是一个实体类，一个实体类里面可以实现多个命令，每个命令是一个单独的方法
#### 开发方法
+ 所有的插件都写在plugins目录下
+ 在插件类上加入<code>@Plugin</code>注解，表示声明这是一个插件
+ 在命令方法上添加<code>@Command(command = "测试")</code>注解，表示这是一个命令处理方法，command表示的是一个命令内容