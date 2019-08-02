　　用于 Tunsafe 实现绕过大陆 IP （类似 ss 的 “绕过大陆地址” 选项）：  
### 用法：  
在 配置文件 的 interface 项最后添加：  
``` 
PreUp = start "" "D:\wireguard\routes-up.bat"
PostDown = start "" "D:\wireguard\routes-down.bat"
```
注意：  这里的 `D:\wireguard\` 为项目文件的路径，路径不允许有中文。  

之后打开 Tunsafe 在 Options 选项中勾选 "Allow Pre/Post Commands"。  