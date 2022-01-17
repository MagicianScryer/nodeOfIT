在浏览器中加载网站时，将分别下载 Javascript 文件和 CSS。您可以通过将两个文件合并为一个文件来优化此过程。该过程可能会增加需要下载的文件大小，但是值得这样做，因为这样做可以节省服务器发出另一个 HTTP 请求的时间。

如何实现：

使用一种特别的写法

```js
<!-- /*
setTimeout('document.body.innerHTML="<span>Hello World</span>"',2000);
<!-- */
<!-- emu{emu:"\
/*"}
span { background-color: #f00; }
span { color: #0ff; }
/* */
```

保存为.css 文件
