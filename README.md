
## UML小组作业
##Github：https://puduio.github.io/PuLiQiong20182123028.github.io/
##     普丽琼 20182123028  

```

****   用例名称： Security System
****   用例说明：
       Adminstrator可以在登录后进行总览、设置安全政策、发布安全公告、查看Dependabot警报、查看代码扫描警报等操作；
       User可以在登录后进行可以在登录后进行总览、设置安全政策、发布安全公告、查看Dependabot警报、查看代码扫描警报等操作；

***    参与者： Adminstrator、User

***    元  素：
                  overview、Scurity advisories、Securitypolicy、Dependbot alerts、Code scanning alerts、
                  view、new dratf security advisory、creat security advisory、start setup、                      
                  Dependbot security updates、sort、automatic detection errors、
                  security analysis from Maketplace.
***    关  系：

                 Adminstrator对于overview、Scurity advisories、Securitypolicy、
                 Dependbot alerts、Code scanning alerts是依赖关系
                 User对于overview、Scurity advisories、Securitypolicy、
                 Dependbot alerts、Code scanning alerts是依赖关系

```
***    建模思路 

       1.	User/Administrator 进入overview之后可以访问Scurity advisories、Securitypolicy
             、Dependbot alerts、Code scanning alerts，所以这些选项和overview是泛化关系。
       2.	User/Administrator 进入Scurity advisories之后可以进行查看公告和编写公告草稿即View
              和new dratf security advisoryd的操作，且当公告编写成功需要发布时可以进行创建新公告的操作
             （creat security advisory）所以View和new dratf security advisoryd和Scurity advisories为
              包含关系，creat security advisory和ew dratf security advisoryd为扩展关系。
       3.	User/Administrator 进入Securitypolicy可以进行设置安全政策的操作（start setup）所以
              Securitypolicy和start setup为包含关系。
       4.	User/Administrator 进入Dependbot alerts可以进行Dependbot security updates、sort操作，
              且只有当需要有文件更新时才发生更新操作，所以Dependbot alerts和Dependbot security updates为扩展
              关系和sort为包含关系。
       5.	User/Administrator 进入Code scanning alerts、可以进行automatic detection errors、security
              analysis from Maketplace.，且Code scanning alerts和automatic detection errors、security analysis
              from Maketplace.为泛华关系。

         


