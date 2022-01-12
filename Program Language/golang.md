# golang

## 实用工具

### 测试

[testify](https://github.com/stretchr/testify) 写断言更方便

[gomonkey](https://github.com/agiledragon/gomonkey) 在写单元测试的时候可以方便的进行函数的替换

### linter

[exportloopref](https://github.com/kyoh86/exportloopref) golang的循环中使用指针，很容易引发意料之外的bug

[prealloc](https://github.com/alexkohler/prealloc) 有些slice可以提前alloc，检查这些slice并给出优化建议

[ifshort](https://github.com/esimonov/ifshort) 查找可以写得更加gopher(意同pythonic)的if语句

[errcheck](https://github.com/kisielk/errcheck) 找出没经过检查的error，给出优化建议

### 代码质量

[gocyclo](https://github.com/fzipp/gocyclo) 计算代码圈复杂度

## 库

[govaluate](https://github.com/Knetic/govaluate) 支持任意c like的表达式解析求解
[bytebufferpool](https://github.com/valyala/bytebufferpool) 字节缓冲池
