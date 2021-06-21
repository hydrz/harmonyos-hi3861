# Hi3861

[`HarmonyOS`](https://gitee.com/openharmony) 开发板 [`Hi3861`](https://device.harmonyos.com/cn/docs/start/introduce/oem_minitinier_des_3861-0000001105041324) 初始化模板

## 前提条件

1. 安装Node.js 12.0.0及以上版本

```
node -v
```

2. 执行如下命令安装最新版本hpm
```
npm install -g @ohos/hpm-cli
```

3. 请先安装Python 3.7.4及以上版本

```
python3 --version
```

4. 安装hb

运行如下命令安装hb

```
python3 -m pip install --user ohos-build
```

设置环境变量

```
vim ~/.bashrc
```

将以下命令拷贝到.bashrc文件的最后一行，保存并退出。

```
export PATH=~/.local/bin:$PATH
```

执行如下命令更新环境变量。

```
source ~/.bashrc
```

执行"hb -h"，有打印以下信息即表示安装成功

```
usage: hb

OHOS build system
positional arguments:
  {build,set,env,clean}
    build               Build source code
    set                 OHOS build settings
    env                 Show OHOS build env
    clean               Clean output
optional arguments:
  -h, --help            show this help message and exit
```

## 开始

1. 安装依赖

```
hpm i
```

2. 打包

```
hpm run dist
```
