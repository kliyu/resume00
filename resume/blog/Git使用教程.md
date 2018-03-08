## Git使用教程   ([博客](http://blog.sina.com.cn/u/5882071529))

使用Git之前，需要先建立一个仓库（repository）。可以使用一个已经存在的目录作为Git仓库货创建一个空白目录。
使用当前目录作为Git仓库，只需使它初始化。

    <span class="hljs-title">git</span> init
    `</pre>

    使用指定目录作为Git仓库。

    <pre>`<span class="hljs-title">git</span> init newre
    `</pre>

    假设在Git仓库根目录下

    ##### 添加新文件

    有一个仓库，但什么也没有，可以使用add命令添加文件。

    <pre>`git <span class="hljs-keyword">add</span> filename
    `</pre>

    ##### 提交版本

    现在已经添加了这些文件，将它们提交到仓库，使它们能够真正的被保存在Git仓库。

    <pre>`<span class="hljs-title">git</span> commit -m <span class="hljs-string">"adding files"</span>
    `</pre>

    git commit命令的-a选项可将所有被修改或者已删除的且已经被git管理的文档提交到仓库中。-a不会造成新文件被提交，只能修改。

    ##### 删除

    如果想从资源里删除文件，使用rm。

    <pre>`git rm <span class="hljs-type">file</span>
    `</pre>

    ##### 分支与合并

    分支在本地完成。要创建一个新的分支，使用branch命令。

    <pre>`<span class="hljs-title">git</span> branch test
    `</pre>

    branch命令知识创建一个新的分支，使用branch命令。

    <pre>`<span class="hljs-title">git</span> branch test
    `</pre>

    branch命令知识创建一个新分支，并不能将我们带入分支。所以我们使用checkout命令来更改分支。

    <pre>`<span class="hljs-title">git</span> checkout test
    `</pre>

    第一个分支，或主分支，被称为"master"

    <pre>`git checkout master
    <span class="hljs-escape">``</span><span class="hljs-escape">`对</span>其他分支的更改不会反应在主分支上。如果想将更改提交到主分支，则需切换回master分支，然后使用合并。
    `</pre>

    git checkout master
    git merge test

    <pre>`如果想删除分支，我们使用<span class="hljs-operator">-d</span>标识。

git branch -d test
```