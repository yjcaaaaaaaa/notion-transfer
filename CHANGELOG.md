# Changelog

## [Unreleased]

- 增加GitHub定时Action

## [0.0.1] - 2022-11-29

### Added

- 实现Notion数据库的初始化，创建所有数据属性关键字
- 实现所有书籍条目到Notion数据库的导入
    - 通过移动端API接口获取主要条目
    - 通过web端html解析获得一些移动端缺失条目，例如ISBN码、价格
    - 解析部分书籍有多种页码
- 实现所有电影条目到Notion数据库的导入
    - 通过移动端API接口获取主要条目
    - 通过web端html解析获得一些移动端缺失条目，例如片长、IMDb码
    - 解析部分演员超过100人问题，仅取前50人
- 数据库条目比对函数
    - 比较新获取条目的信息，比对以下内容如果发生变化就更新条目
        - 标记状态
        - 标记时间
        - 个人评分
        - 类型标签 🏷️

### Changed

- 更新显式时区信息对齐
