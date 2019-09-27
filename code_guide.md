# 代码规范

### 1.类名

#### 1.1 通用
规则：模块名+功能名+类型   
示例：LoginActivity、FileUtils
#### 1.2 特殊
- AbstractLogin
- BaseView
- LoginActivityTest
- *interface*  
  - Runnable、Accessible  
  - OnClickListener
  - IBinder

### 2.变量名

#### 2.1 通用
- static final -> CONSTANT_NAME
- static -> sApplication
- non-static、non-public -> mFied
- non-static、public -> fied

#### 2.2 特殊
- *java bean*  
LowerCamelCase, boolean类型无需加前缀is
- *acronym(首字母缩略词)*   
当做一个word对待  
示例：XmlHttpRequest、supportIpv6OnIos


### 3.资源

#### 3.1 资源文件名
##### 3.1.1 anim
- 补间动画  
规则：类型+方向  
示例：fade_in、push_left
- 其他  
模块名+描述

##### 3.1.2 drawable  
规则：类型+描述+状态  
示例：btn_send_normal、ic_star、dialog_top
##### 3.1.3 layout
规则：类型+描述  
示例：activity_main、item_person、partial_status_bar
##### 3.1.4 mipmap
只存放应用图标
##### 3.1.5 vaules
规则：类型的复数形式  
示例：strings.xml、dimens.xml、attrs.xml

#### 3.2 资源id和name名
##### 3.2.1 id
规则：类型+模块+描述   
示例：tv_name、tv_login_name
##### 3.2.2 name
规则：模块+描述  
style类型为UpperCamelCase,其他类型为下划线小写  
示例：title_content、login_title_content
