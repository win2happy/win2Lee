## HaxExtend with Github Action
#### 计划
- [Helium](https://github.com/mybdye/HaxExtend_helium) 版本研究中

#### 更新
- 0328 增加了一丢丢 delay
- 0326 基本框架完成
- 0324 Selenium 学习

#### Secret 增加以下变量
- ```USERNAME```
- ```PASSWORD```
- ```BARKKEY``` (可选)

#### 触发方式
默认手动+cron，每三天早上 8/9/10 点执行

```
/.github/workflows/main.yml
```

```
on:
  #push:
  schedule:
    # run every 3 days on UTC 0/1/2am (8/9/10am CN time)
     - cron: '0 0,1,2 */3 * *'
  # Allows you to run this workflow manually from the Actions tab
  workflow_dispatch:
```

#### ```随缘 Extend，Possibly blocked by google```

<img src=./result.jpeg width=50% />

#### 参考
- https://www.python.org/
- https://www.selenium.dev/
- https://www.youtube.com/watch?v=As-_hfZUyIs
- https://github.com/actions/virtual-environments/blob/main/images/macos/macos-12-Readme.md
