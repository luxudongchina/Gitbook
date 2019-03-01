# 贡献格式

1. 自行编撰
```
# 第一行为维护者信息
Maintainer: 姓名 学号 <邮件地址/其他联系方式>
# 若不想维护,按如下填写
Contributor: 姓名 学号 <邮件地址/其他联系方式>
# 第二行为添加的章节,如果没有分章节,请写 "+0"
# 以后修改直接接在这一行后面.
+1~7 (添加了1~7个章节)
# 也可以写成
+1, +2, +3, +4, +5, +6, +7
```
2. 修改者
```
# 追加在最后, 如果没有维护者有准备维护,填写自己为 "Maintainer"
Contributor: 姓名 学号 <邮件地址/其他联系方式>
# 第二行为添加,修改和删除的章节,请分章节描述
# "+" 为增加, "-" 为删除, "=" 为修改
+8, -1 =2
```

3. 工作量证明的patch生成方法
```
git diff <from> <to>
```

例子
````
diff --git a/chapter2.md b/chapter2.md
index 4f5f845..3992afb 100644
--- a/chapter2.md
+++ b/chapter2.md
@@ -2,25 +2,25 @@

 当所需工具安装好之后，就可以进行写书工作了，这个过程还是比较简单的。具体过程如下：

-1、需要在[GitHub](https://github.com/)下建一个仓库，仓库名建议和本地书籍准备存放的目录名一致。
+1. 需要在[GitHub](https://github.com/)下建一个仓库，仓库名建议和本地书籍准备存放的目录名一致。

-2、Gitbook Editor是一个图形化界面的工具，应该很快就能学会编辑一本书籍。
+2. Gitbook Editor是一个图形化界面的工具，应该很快就能学会编辑一本书籍。

-3、需要时，可以通过push或sync操作将本地所写的书籍源码，同步到GitHub相应仓库的Master分支。（需要输入GitHub的账号和密码）
+3. 需要时，可以通过push或sync操作将本地所写的书籍源码，同步到GitHub相应仓库的Master分支。（需要输入GitHub的账号和密码）

-4、多人协作时，和GitHub配合，用pull，push，sync等命令，完成书籍的协同编辑工作。
+4. 多人协作时，和GitHub配合，用pull，push，sync等命令，完成书籍的协同编辑工作。

-5、在书籍所在目录下，利用下述命令生成书籍的 html 格式，存放路径为所在目录下的子目录\_book。
+5. 在书籍所在目录下，利用下述命令生成书籍的 html 格式，存放路径为所在目录下的子目录\_book。

 ```
 gitbook build
 ```

-6、继续使用下面的_ _命令将生成的\_book目录下内容push到对应仓库的gh-pages分支下。
+6. 继续使用下面的_ _命令将生成的\_book目录下内容push到对应仓库的gh-pages分支下。

 ```
 gh-pages -d _book
 ```

-7、现在已经可以访问了。访问路径为 [https://&lt;username&gt;.github.io/&lt;project&gt;。](https://<username>.github.io/<project>。)
+7. 现在已经可以访问了。访问路径为 [https://&lt;username&gt;.github.io/&lt;project&gt;。](https://<username>.github.io/<project>。)

````
