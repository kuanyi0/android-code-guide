# 项目规范

### 1.包名

#### 1.1 前3级包名
规则：com(net...).个人/公司名.应用名  
示例：com.yikuan.application  

#### 1.2 第4级包名

##### 1.2.1 Package By Layer
- base
- ui
  - activity
  - fragment
  - widget
- service
- receiver
- provider
- data
- adapter
- ...
- util
- *XxApplication*
- *Constant*

##### 1.2.2 Package By Feature
- base
- ui
  - activity
  - fragment
  - widget
- service
- receiver
- provider
- data
- adapter
- feature1
- ...
- feature2
- util
- *XxApplication*
- *Constant*

##### 1.2.3 说明
PBF:   
feature包属于私有，包含相关的类(XxActivity、XxUtils...)  
其他的包均属于公有，包含公共的类(BaseActivity、LogUtils...)