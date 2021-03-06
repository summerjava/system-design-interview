# 大厂系统设计面试真题
## 系统设计面试步骤指引  
[大厂系统设计面试步骤指引](https://github.com/xiajunhust/system-design-interview/blob/main/%E5%A4%A7%E5%8E%82%E7%B3%BB%E7%BB%9F%E8%AE%BE%E8%AE%A1%E9%9D%A2%E8%AF%95%E7%9C%9F%E9%A2%98/%E7%B3%BB%E7%BB%9F%E8%AE%BE%E8%AE%A1%E9%9D%A2%E8%AF%95%E6%AD%A5%E9%AA%A4%E6%8C%87%E5%BC%95.md)
## 分布式ID的生成  
常见如交易号等都需要生成分布式唯一ID。  
思路：  

- 利用mysql的自增机制。
- 利用开源项目Twitter Snowflake，需要了解下其核心算法实现。

## 类似新浪微博短链接系统设计  
思路：采用发号策略，对应每一个长链接，生成一个唯一的号码，拼接成短连接。  
需要考虑的问题：  

- 发号器的设计。小系统可以直接用数据库MySQL的自增。考虑高并发的话可以用如redis做发号器。
- 发号器的高可用。
- 短链接的存储。

## Instagram的数据存储  
思路：数据分片，主要是分片ID的设计。

## K-V存储引擎  
思路：可以参考开源的Rocksdb和LevelDB。

## 网络爬虫  


---

致力于分享干货，为每一位计算机CS学子学习道路上带来帮助。

也欢迎大家关注我的公众号「编程学习指南」，***获取更多计算机干货~提供大厂（阿里、字节、美团、快手、网易等）内推、简历修改、面试咨询、毕设咨询等服务***。

![欢迎大家关注我的公众号](https://github.com/xiajunhust/awosome-cs/blob/main/QR-CODE.jpg)

