# 基于 SIFT 算法的全景拼接软件

---

## 介绍

本软件分为命令行版本以及图形用户界面版本。

- 命令行版本

- [图形用户界面版本](https://github.com/AnNingUI/GetPanorama)

  - 基于 vue-pywebview-pyinstaller 二次开发

- 构建指令

```bash
# 国内用户请自行切换镜像，不然会下载的很慢
# 插件虚拟环境
python -m venv .venv

# 进入虚拟环境
./.venv/Scripts/activate

# 开始构建 Linux or MacOs
bash ./build.sh
# 开始构建 Windows
./build.bat
```

---

<div class="annotation-container">
  <span class="text">注：</span>
  <div class="box">图片集所需图片尽量小于或等于三张【<span class="text-important">可以尝试多次拼接</span>】</div>
  <div class="box">尺寸尽量小于或等于1920*1080【<span class="text-important">使用压缩工具或项目脚本(minisize.py)</span>】</div>
  <div class="box code">python minisize.py -i path -wh 1920,1080</div>
  <div class="box">第二次拼接不要存在上一次路径【<span class="text-important">未开发hash命名功能</span>】</div>
</div>

---

## 致谢

- [skimae](https://github.com/scikit-image/scikit-image)
