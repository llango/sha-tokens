# Shallot Tokens

修改Mozilla的Protocol, 用于火葱设计系统。

<em>JavaScript · JSON · CSS · SCSS</em>

---

## 信息

<table>
<tr>
<td>包名</td><td>@llango/tokens</td>
</tr>
<tr>
<td>描述</td>
<td>修改Mozilla的Protocol, 用于火葱设计系统</td>
</tr>
<tr>
<td>版本</td>
<td><a href="https://github.com/llango/sha-tokens/blob/master/CHANGELOG.md">1.0.3</a></td>
</tr>
</table>

## 安装

该设计tokens包可以使用 npm 安装。(`sha-tokens`) [npm](https://www.npmjs.com/package/sha-tokens).


### JavaScript 包安装

使用 [npm](https://www.npmjs.com/):

```
npm install sha-tokens --save
```

使用 [yarn](https://yarnpkg.com/en/):

```
yarn add sha-tokens
```

### JavaScript

在JavaScript中，tokens设计采用[lower camelCase](http://wiki.c2.com/?CamelCase)格式化。

```js
const tokens = require('sha-tokens/dist/index');
console.log(tokens.colorBlueLighter); // rgb(0, 0, 0)
```

In JSON, tokens设计采用 [kebab-case](http://wiki.c2.com/?KebabCase)格式化。

```js
const tokens = require('sha-tokens/dist/index.json');
console.log(tokens['color-black']); // rgb(0, 0, 0)
```

### Sass

Sass 变量和匹配键采用 [kebab-case](http://wiki.c2.com/?KebabCase)格式化。

```scss
// Using variables
@import 'sha-tokens/tokens/dist/index';

a {
  color: $color-black;
}
```

### Sass, 和 CSS 自定义属性

自定义属性采用 [kebab-case](http://wiki.c2.com/?KebabCase)格式化。

```scss
// Omit .css at the end of the file
@import 'sha-tokens/dist/colors/colors.custom-properties';

a {
  color: var(--color-black);
}
```

## 发布

要发布到npmjs注册表，你需要访问npmjs.com上的rontomai。 首先运行`gulp`在本地编译包。你可以查看本地的`dist`文件夹，以验证它具有最新的token。然后运行`npm publish` 进行发布。

## 贡献

欢迎贡献。

