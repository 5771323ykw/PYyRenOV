# 前言

随着我国对环境保护的日益重视，垃圾分类成为了一种新兴的生活方式。为了鼓励和引导大众积极参与垃圾分类，我们开发了基于SSM（Spring、Spring MVC、MyBatis）的垃圾分类奖励系统。通过此系统，用户可以便捷地参与到垃圾分类活动中，并获得相应的积分奖励。以下是关于本项目的详细介绍。

# 内容介绍

本项目是一款基于Java语言的垃圾分类奖励系统，采用Spring、Spring MVC和MyBatis框架进行开发，前端技术包括JS、Vue和CSS3。系统主要包括用户注册登录、垃圾分类知识学习、垃圾分类行为记录、积分奖励等功能。通过该项目，我们希望能为广大用户提供一个便捷、实用的垃圾分类工具，提高大家的环保意识。

# 技术介绍

- 语言：Java
- 使用框架：Spring、Spring MVC、MyBatis
- 前端技术：JS、Vue、CSS3
- 开发工具：IDEA/Eclipse
- 数据库：MySQL 5.7/8.0
- 数据库管理工具：phpstudy/Navicat
- JDK版本：jdk1.8
- Maven: apache-maven 3.8.1-bin
- 前端环境：Node.Js 12\14\16

# 核心代码

以下是本项目中的一个核心代码片段，展示了用户积分增加的逻辑：

```java
@Service
public class ScoreService {

    @Autowired
    private ScoreMapper scoreMapper;

    // 增加用户积分
    public void addScore(Integer userId, Integer score) {
        Score userScore = scoreMapper.selectByUserId(userId);
        if (userScore == null) {
            userScore = new Score();
            userScore.setUserId(userId);
            userScore.setScore(score);
            scoreMapper.insert(userScore);
        } else {
            userScore.setScore(userScore.getScore() + score);
            scoreMapper.updateById(userScore);
        }
    }
}
```

# 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img12.360buyimg.com/ddimg/jfs/t1/332460/23/11309/181187/68c05ddbFa3cbc769/b554d8cb3e3f129d.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/333444/38/11145/26757/68c05db9Fb56199bf/a327079129bb55ca.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/342693/29/1508/132225/68c05dbbFf3dccd3e/d8c5e902d56b2820.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/346948/33/1530/24050/68c05dbcFf3f9a6c2/bd64d9567acffa39.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/326047/10/18217/25427/68c05dbcFce2496f5/8d2c2b49dad4a246.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/337962/28/8731/23233/68c05dbdF69246fed/93d978af38202e56.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/339757/39/8965/79137/68c05dbeFabfa8c84/990125f32f2750d1.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/349702/6/1571/119125/68c05dbeF0257457c/84f2c86e17cd026c.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/324549/28/18119/37774/68c05dbfFdb9d0783/2ed54dd3901e10b4.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/341834/2/1546/53953/68c05dbfFb85900e9/2f9a5851da0cffc6.jpg)

