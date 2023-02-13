# jquery-affictoc

## 一、介绍

jquery-affictoc 是一款生成文章目录的插件

## 二、使用方式

```javascript
<div class="left">
    <div class="info">
        <ul>
            <li>主页</li>
            <li>归档</li>
            <li>分类</li>
            <li>标签</li>
            <li>动态</li>
            <li>关于</li>
        </ul>
    </div>
    <div class="toc-panel">
        <div class="toc-container"></div>
    </div>
</div>
<div class="right">
    <div class="post-panel">
        <div class="post-content">
          ......
        </div>
    </div>
 </div>   
<script src="jquery.min.js"></script>
<script src="jquery.affixtoc.js"></script>
<script>
    $(".toc-container").affixToc({
        affixEle: ".toc-panel",    // 需要固定的容器
        scopeEle: ".post-content", // 搜索文章标题的容器
        offset: 190,               // 滚动到当前值就固定容器
        activeColor: "#234ce5"     // 目录标题被激活的颜色字体
    });
</script>
```


