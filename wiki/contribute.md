# 参与贡献 Wiki

我们采用 [Docsify](https://docsify.js.org) 。

源文件存放于 [GitHub](https://github.com/thisaccn/wiki)。

### 参与要求 :id=required

- 了解 Markdown 语法。
- 了解 Git 的基本用法。
- 有较好的文字表达能力。
- 了解红石云社区和服务器的内容。

### 参与方式

##### 加入 Collaborators

如果你能够熟练使用 Git 和 Markdown 语法，并且能灵活处理各种路径和文件问题，即可以申请加入 Collaborators 获得直接写权限。

向红石云工场管理团队申请加入本 repo 的 Collaborators，确认邀请后即可直接编辑 repo 内的文件。

##### 提交 P R

如果你尚不熟悉 Git 操作或 Markdown 语法，但是希望参与贡献，可以 fork 本 repo 来编辑。

完成后，访问本 repo 并提交 Pull Request (PR)。协作者将 review 所有变更，如无问题，即可合并进本 repo。

### 文件结构

- `index.html` - 用于导入 Docsify，并包含 Docsify 的各项参数，如无必要请勿修改。
- `README.md` - Wiki 主页内容。
- `_navbar.md` - 导航栏，如无必要请勿修改。
- `_sidebar.md` - 侧边栏，如果新增较重要的页面可在这里做相应的修改。
- `_404.md` - 404 页面，如无必要无需修改。
- `changelog.md` - 服务器重大变更记录。一年以上的需归档至`changelogs`目录。
- `assets` - 各种静态文件目录。
  - `css` - 为本Wiki定制的样式规则。
  - `images` - **图片存放处。**如需内部引用图片，请先复制至此。
- 分类目录说明
  - `changelogs` - 服务器于当年以前的变动，以及民间事件（`unofficial-events.md`）。
  - `legacy` - 归纳“过时页面”，仅用于历史考古。
  - `subserver` - 子服务器相关内容。
  - `works` - 红石云工场的各项设定、规划区、经济、工程、特色物品和活动等等。
  - `space` - 玩家产生的服务器相关艺术作品，包括绘画、游戏内合影、音视频等。
  - `tutorial` - 玩家贡献的各种教程。
    目前包含建筑教程、交通导航、插件（命令）帮助三大项。
  - `wiki` - 各类基础信息，规则、说明性文本等。
    其中《基本规则》《白名单申请》仅由管理组编辑。
  - `misc` - 其它未归类信息的临时存放处，不宜长期使用。
- 如果有额外的详细信息页面，还可以在以上对应目录中新建目录来整理。

### 编辑说明 :id=editing-notes

1. **所有文本都必须使用 UTF-8 编码**。
2. 编辑或新建页面时，应保持文件结构正确、整洁。
3. 文件和目录命名保持简洁，文件名应只包含英文、数字、短线（`-`）。
4. Wiki 内的链接应使用相对路径，并注意检查引用路径是否正确。
5. 文本排版保持简洁、美观。中文和西文、数字之间要有空格。
6. 请勿滥用 heading 语法。推荐：
   - 页首标题使用一级 heading；
   - 章节/section 使用三级 heading（如希望侧边栏自动展开 table of contents，则需要使用二级 heading）；
   - 小节使用四、五级 heading。
   - 为方便引用及跳转，可将章节标题编辑成 `## 标题 :id=required` （其中 `required` 可替换为任意内容）。  
   此后，引用该章节仅需 `[像这样](#required)` 设置链接，例如在本页转到[参与要求](#required)。  
   如在其它页面引用该章节，`[可以这样](wiki/contribute#required)`。
7. 并不是所有的页面都要列入侧边栏。一些详细内容的页面也可以存放在相应目录下并通过其他页面访问。
8. 本Wiki源仓库托管于 GitHub，为确保拉取、推送顺畅，应尽量避免上传文本以外的文件。  
  对于图片，有条件者应尽量引用外链；确需由Wiki自行托管的，应先尽可能压缩图片，推荐通过[Jpgmin](https://jpgmin.cn)压缩。  
  对于非图片文件，请使用稳定可靠的文件托管外链服务。
9. Docsify 可能与你所用 Markdown 编辑器**存在分歧**。为避免过多的 commit，请先在本地运行 Wiki 预览效果。
   - 如使用 VS Code，可以安装插件 [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)，然后点击右下角的 **Go Live**，用浏览器访问 `localhost:5500` 即可预览。  
   - 对于其它情况，可运行 `docsify serve`，然后浏览`localhost:4000`。
10. 所有 commit 的备注内容都将公开于众，为便于跟踪与更正，应如实概括所作变更，并避免加入任何无关信息。


### 相关链接

* [Docsify 的特有文档语法](https://docsify.js.org/#/helpers)
* [Jpgmin](https://jpgmin.cn)——Mozjpeg 与 PngQuant 的第三方网页界面，压缩效果好，可批量压缩，操作简便。
