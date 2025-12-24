# 为什么启动不了客户端

可能是被：`WSL2 / Hyper-V 动态保留（最常见！）`  
需要关闭动态分配：管理员CMD运行 `reg add "HKLM\SYSTEM\CurrentControlSet\Services\hns\State" /v EnableExcludedPortRange /d 0 /f`  
然后重启电脑，然后再次打开软件