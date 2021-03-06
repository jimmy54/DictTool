# DictTool 词库处理工具


## 本项目使用GPLv3开源协议

## 作者对版权的额外强调

您可以免费并且在不通知作者的情况下，使用和修改本项目，但是要遵守如下规则：
<br>1 您不能在您的软件为闭源软件时包含此项目的任何内容。
<br>2 您不能在收费软件中包含此项目的任何内容。
<br>3 您使用修改后的本项目代码，但必须明确标记原作者及项目的版权信息。
<br>4 您可以免费使用此项目，但您不能删除项目中包含的任何作者或版本信息。


# 功能模块

注：本工具使用打散格式作为本工具通用格式，除格式转换模块，其它模块的输入词库格式都是打散格式
<br>格式参考
<br>f 地
<br>f 土
<br>fbgf 地球
<br>g 一
<br>g 王
<br>ytyt 谢谢
<br>……



## 格式转换

### QQ格式→打散格式（本工具格式）
说明略
<br>
<br>QQ格式参考
<br>f 地 土
<br>fbgf 地球
<br>g 一 王
<br>ytyt 谢谢
<br>……

### 多多格式→打散格式（本工具格式）
说明略
<br>
<br>多多格式参考
<br>地&lt;tab&gt;f
<br>土&lt;tab&gt;f
<br>地球&lt;tab&gt;fbgf
<br>一&lt;tab&gt;g
<br>王&lt;tab&gt;g
<br>谢谢&lt;tab&gt;ytyt
<br>……

### 打散格式（本工具格式）→QQ格式
说明略

### 打散格式（本工具格式）→多多格式
说明略


## 查询检测工具

### 字符编码检测
检测输入字符的Unicode和UTF-8编码

### 按键编码检测
检测按键编码

### 重码情况检测
对词库进行重码统计


## 词库简单处理

### 排序词条
对词库根据编码进行排序

### 反转词条顺序
把词库顺序进行反转，比如原来是从a到z，就变成从z到a
<br>a 工
<br>b 了
<br>c 以
<br>--↓--
<br>c 以
<br>b 了
<br>a 工

### 交换编码与候选
交换编码与候选的位置
<br>a 工
<br>b 了
<br>c 以
<br>--↓--
<br>工 a
<br>了 b
<br>以 c

### 去重合并词库
a 工
<br>a 工
<br>b 了
<br>--↓--
<br>a 工
<br>b 了

### 提取字词或排除字词
根据参考词库做交集或并集

### 去除候选唯一
为唯一候选增加空候选，来去除指定码长的候选唯一（用于不能取消四码唯一自动上屏的五笔输入法等）


## 词库高级处理

### 制作出简不出全词库
a 工
<br>aa 工
<br>aaaa 工
<br>b 了
<br>c 以
<br>--↓--
<br>a 工
<br>b 了
<br>c 以

### 提取指定长度的词条
根据参数提取符合条件的词条

### 生成词条编码
根据用户给定的规则生成字/词的编码

### 编辑词条编码
根据用户给定的规则修改字/词的编码

### 制作百度手机输入法自定义方案
制作百度手机输入法的def格式导入文件

### 制作QQ五笔导入文件
根据用户的词库，分离词库成为系统词库txt和自定义短语txt（防止系统词库不能导入非普通中文的候选内容）
