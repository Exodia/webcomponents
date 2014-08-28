WebApps WG -- Web Components
===============

This is the repository in which W3C editor's drafts of the Web Components specs are maintained.

- [Introduction to Web Components](http://w3c.github.io/webcomponents/explainer/).
- [Shadow DOM](http://w3c.github.io/webcomponents/spec/shadow/).
- [HTML Imports](http://w3c.github.io/webcomponents/spec/imports/).
- [Custom Elements](http://w3c.github.io/webcomponents/spec/custom/).

## 翻译须知

我们翻译的方式是先翻译目前官方 [github](https://github.com/w3c/webcomponents) 的最新版本。
具体方式是把官方 [github](https://github.com/w3c/webcomponents) 的最新版本派生到一个新的 `zh` 分支，并在这个分支下进行翻译。

### 参与翻译的方式

**为了避免冲突，请务必在翻译之前，在 [issues](https://github.com/w3c-html-ig-zh/webcomponents/issues) 里创建一个 issue，说明你翻译的范围**

在项目首页 **fork** 项目，然后 checkout 到 `zh` 分支，修改相应的文件，翻译好之后记得 commit、push、然后发起从你自己的 `zh` 分支到我的 `zh` 分支的 merge request。

为了保证翻译质量，文档全部翻译完成之后，需要进行至少 2 轮的交叉 review。

#### `zh` 分支新产生的文件及其对应关系

```
webcomponents
├─┬ explainer
│ └── index.html
├─┬ explainer-zh
│ └── index.html 新的 web components 介绍的翻译
├─┬ spec
│ ├─┬ custom
│ │ └── index.html
│ ├─┬ imports
│ │ └── index.html
│ └─┬ shadow
│   └── index.html
└─┬ spec-zh
  ├─┬ custom
  │ └── index.html 新的 custom elements 的翻译
  ├─┬ imports
  │ └── index.html 新的 html imports 的翻译
  └─┬ shadow
    └── index.html 新的 shadow dom 的翻译
```

### 后续维护

每次翻译更新/结束之后，给版本打一个 tag，并合并到 `gh-pages` 分支。

由于 web components 规范还在不断的迭代完善之中。所以今后我们会不定期把官方 [github](https://github.com/w3c/webcomponents) 的改动合并到我们的 `zh` 分支 (由于我们不修改原有的文件，只产生新的翻译文件，所以除了 `README.md` 文件本身是不可能有冲突的)，同时用 `diff` 工具找出版本之间的差异，再把这些收集到的差异体现在翻译上，生成新的翻译的版本。

