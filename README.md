# vue-separator

## input框分隔符功能描述：
1. 在输入框中使用键盘输入数字，输入框中的数字自动被 `-` 分隔。例如在输入框中输入 `123`, 则输入框自动变成 `1-2-3`。
2. 需要考虑移动光标在中间输入之后的光标问题。例如输入框中已经显示 `1-2-3`, 此时将光标移动到 `2` 的后面继续输入，光标不能被自动移到最末尾。删除操作同理。
3. `-` 号与数字的数量一一对应。例如有3个数字 `1-2-3`，则 `-` 也必须为3个。

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
