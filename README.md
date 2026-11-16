# 文本差异对比（手机版）

lzltool.cn/contrastdiff 同款核心引擎（Monaco Editor 0.52.2，微软官方 npm 包，MIT），外壳重写为手机友好版。

## 功能

- 双栏并排，直接在栏内粘贴/输入，差异实时标出（红删绿增、字级高亮）
- 行号以行数多的一侧为准，两侧对齐
- 单栏/并排切换、折叠相同代码、忽略行首尾空白、自动换行
- 语言高亮：CSS / JS / JSON / HTML / XML / YAML / SQL / Java / Python / 纯文本
- 整页上下滚动，无内部滚动条；防手机浏览器误缩放

## 部署到 GitHub Pages

1. 新建仓库（公开），把本目录全部内容（index.html + monaco/ 文件夹）传到仓库根目录
2. 仓库 Settings → Pages → Source 选「Deploy from a branch」，Branch 选 main / 根目录 (root)，保存
3. 等 1-2 分钟，访问 `https://你的用户名.github.io/仓库名/`

注意：monaco/ 必须原样保留（懒加载按文件路径取），不要合并进单文件、不要改路径。

## 本地运行

必须有 http 访问，直接双击 file:// 打不开（浏览器 worker 限制）：

```
python3 -m http.server 8899
# 浏览器打开 http://127.0.0.1:8899
```
