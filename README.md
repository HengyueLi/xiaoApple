# xiaoApple (小苹果)

跨平台，轻量级的阿里云盘同步工具。简单易用。造个轮子自己用...(-_-)


# 安装

```
pip install xiaoApple
```

# 例子

```python


import xiaoApple

localDir = r"c:\users\admin\desktop\syncdir"
aliDir = 'syncdir' 
apple = xiaoApple.Sync(localDir,aliDir)


# 单次同步。如果文件很多，第一次很慢...
apple.run()


# # 自动间隔720秒同步一次
# apple.auto(syncCycleSec=720) 


# # 列出最近的删除备份，可用于恢复数据
#  print(apple.listDelteBackups())


# # 根据listDelteBackups得到的列表，可以根据备份恢复删除的文件
# apple.recoverBackup('2024-11-12T082104')



```

# 参数配置

有一些，以后再写...