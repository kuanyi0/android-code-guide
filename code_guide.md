# 代码规范

### 1.命名基础
#### 1.1 通用
- 类名：UpperCamelCase
- 方法名：LowerCamelCase
- 常量名：CONSTANT_CASE
- 变量名：LowerCamelCase
#### 1.2 特殊
- *acronym（首字母缩略词）*
当做一个word对待  
示例：XmlHttpRequest、supportIpv6OnIos
#### 1.3 说明
- 常量  
内容不可变的成员变量，static final修饰的不一定是常量

### 2.类名
#### 2.1 通用
规则：模块名+功能名+类型   
示例：LoginActivity、FileUtils
#### 2.2 特殊
- AbstractLogin
- BaseView
- LoginActivityTest
- *interface*  
    - Runnable、Accessible  
    - OnClickListener
    - IBinder


### 3.成员变量名
#### 3.1 通用
- static -> sApplication
- non-static、non-public -> mFiled
- non-static、public -> filed
#### 3.2 特殊
- *java bean*  
LowerCamelCase，boolean类型无需加前缀is
- 使用kotlin时，无需加前缀


### 4.资源
#### 4.1 资源文件名
##### 4.1.1 anim
- 补间动画  
规则：类型+方向  
示例：fade_in、push_left
- 其他  
模块名+描述
##### 4.1.2 drawable  
规则：类型+描述+状态  
示例：btn_send_normal、ic_star、dialog_top
##### 4.1.3 layout
规则：类型+描述  
示例：activity_main、item_person、partial_status_bar
##### 4.1.4 mipmap
只存放应用图标
##### 4.1.5 values
规则：类型的复数形式  
示例：strings.xml、dimens.xml、attrs.xml
#### 4.2 资源id和name名
##### 4.2.1 id
规则：类型+模块+描述   
示例：tv_name、tv_login_name
##### 4.2.2 name
规则：模块+描述  
style类型为UpperCamelCase，其他类型为下划线小写
示例：title_content、login_title_content

### 5.注释
#### 5.1 类注释
规则：必须写明作者和时间  
示例：
```
@author yikuan
@date 2020/05/20
```
#### 5.2 方法注释
示例：
```
/**
 * view 转 bitmap
 *
 * @param view view 对象
 * @return bitmap
 */
```
#### 5.3 块注释
示例：
```
// This is a comment.
```
#### 5.4 特殊注释
规则：使用//、-、+、｜符号  
示例：
```
//-----------------------
// This is a comment
//-----------------------
```
```
//-----+-----+-----+-----
//  0  |  1  |  2  |  3
//-----+-----+-----+-----
//  4  |  5  |  6  |  7
//-----+-----+-----+-----
```