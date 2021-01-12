---
title: "Go-反转字符串函数"
date: 2020-11-30T14:52:24+08:00
draft: false
toc: true
url: "/technology/2020/11/30/tech01"
categories: 
- 技术
tags: 
- go
- golang
---
## go反转字符串函数
```
    package main
    import "fmt"
    func reverse(str string) string {
        var result string
        strLen := len(str)
        for(i := 0; i < strLen; i++){
            result = result + fmt.Sprintf("%c", str[strLen-i-1])
        }
        return result
    }
    
    //调用
    result := reverse("hello world")
    fmt.Println(result)
    //结果    dlrow olleh
```