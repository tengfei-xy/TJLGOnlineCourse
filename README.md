# TJLGOnlineCourse
当代年轻人刷网课方式！注：适用天津理工大学成人本科的网课学习平台！

## 一、项目说明

该项目是一种通过命令行（macOS、Linux）来学习网课的方式。后台自动完成观看所有视频（完成时间取决于学习时长）。

> 注：Windows不支持使用，除非在windows安装bash/zsh的执行环境



## 二、video.sh脚本说明

### 2.1 变量说明

将脚本使用之前需要修改的变量是

**header_cookie**：登录网课后，即可通过浏览器获取到Cookie

**sleep_time**：睡眠时间，指定30，大于30的值毫无意义

> 参考格式：
>
> header_cookie="Cookie: .CHINAEDUCLOUD=; _pk_testcookie.540.b662=; _pk_id.540.b662="
>
> sleep_time=30

## 2.2 使用说明

1. 如果一节课程（包括其下的小节课）全部学习完成，将跳过学习

2. 该脚本将重复执行，直到所有课程全部完成。下方是全部学习完成的日志输出

   > 姓名:xx
   >
   > 课程:中国近代史纲要 已完成
   >
   > 课程:会计学 已完成
   >
   > 课程:大学英语 已完成
   >
   > 课程:数据库技术及应用 已完成
   >
   > 课程:毛泽东思想和中国特色社会主义理论体系概论 已完成
   >
   > 课程:管理学 已完成
   >
   > 课程:经济数学 已完成
   >
   > 所有课程学习完毕

3. 并没有手动验证窗口以及IP判断，保存学习进度的get请求只需要保证cookie即可



## 三、联系方式

对脚本使用用疑问，欢迎交流，联系方式位于[个人首页](https://github.com/tengfei-xy)
