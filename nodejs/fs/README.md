## fs 文件系统

### 1、fs.readdirSync(path[, options])

- path: 名称或路径

```js
const files = fs.readdirSync(name);
console.log(files);

// 输出
["README.md", "index.js"];
```

### 2、fs.readFileSync

```js
const content = fs.readFileSync("index.js");
console.log(content);

// 输出
//<Buffer 65 78 70 6f 72 74 20 7b 20 64 65 66 61 75 6c 74 20 7d>

const content = fs.readFileSync("index.js").toString();
const content = fs.readFileSync("index.js", {
  encoding: "utf-8",
});
// 输出
// export default {};
```

### 3、fs.existsSync

存在，返回 **true**；不存在，返回**false**


