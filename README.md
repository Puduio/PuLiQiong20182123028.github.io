
## UML小组作业

##Github：https://puduio.github.io/PuLiQiong20182123028.github.io/

##     普丽琼 20182123028  

##     第二次作业
```
1）．试论述类与用例的区别。
答案:类是对一组具有相同属性，操作、关系和语又的对象的描述。类是对事物的抽象。而用例是对一组序列动作的描述，系统执行这些动作将对用例的参与者产生可以观察的结果。

2）．试比较边界类与实体类的异同。
答案:实体类是对系统中需要存储的信息和其信息的行为建立模型。实体类具有永久的特性，这类似于数据库中的表一样用于保存系统的业务信息。
边界类位于系统与外界的交接处，它在一个或多个角色和系统之间建立相互作用的模型。

3）．试运用本节所学的静态建模技术找出用户管理模块中的所有的类。
用户类、用户管理界面类、数据库操作类、管理员类、

4）．请找出学生管理系统中学生注册用例的实体类，边界类，控制类。
实体类：学生类；
边界类：注册界面类；
控制类：注册类，对应的是用例中的注册。

5）．什么是依赖？它与关联有什么区别？
答案:依赖是一种使用关系，它说明了一个事物声明说明的变化可能影响到使用它的另一个事物，但反之未必。也就是说，服务的使用者以某种方式依赖于服务的提供者。而关联是一种结构关系，它详述了.一个事物的对象与另一个事物的对象相互联系。

6)．什么是泛化？泛化是否就是类的继承，如果不是请说明理由。
答案:泛化是一般事物(称为父类或超类)和较特殊事物(称为子类或孩子类)之间的关系。泛化不是类的继承，类的继承是泛化的一种。

7）．试论述聚合和组合的异同。
答案:聚合描述了整体对象拥有部分对象的关系。组合是聚合的一种形式，它具有强的拥有关系，而且整体与部分的生命周期足一致的。


```
## 第一次作业

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
              from Maketplace.为泛化关系。
```
![image](https://github.com/Puduio/PuLiQiong20182123028.github.io/blob/main/Untitled.mdj)
         


