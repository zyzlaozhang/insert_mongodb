# 导入方法
```cmd
pip install insert_mongodb
```
# **注意事项**

要导入的**json**文件为**下面**的格式
```json
[
{"xxx":"xxx"},
["xxx","xxx"]
]
```

**小贴士**

搭配*mongodb_to_other*库使用更加 

***注意***

使用本库但是**函数选择错误**者，若**数据丢失**，我**概不负责**

## 1.Import_different_items函数

### 1.1导入
```python
from insert_mongodb import Import_different_items
    #倒库
Import_different_items("数据库","集合名","要导入的文件路径",port=int('数据库端口(默认为27017)'),ip="mongodb数据库所在的ip地址(默认为127.0.0.1)",name="数据库用户名(默认为None)",password="数据库密码(默认为None)")

```
### 1.2 功能详解
导入在mongodb中**不存在**的集合并且**保留原数据**

## 2.Import_retain_different_items函数

### 2.1导入
```python
from insert_mongodb import Import_retain_different_items
    #倒库
Import_retain_different_items("数据库","集合名","要导入的文件路径",port=int('数据库端口(默认为27017)'),ip="mongodb数据库所在的ip地址(默认为127.0.0.1)",name="数据库用户名(默认为None)",password="数据库密码(默认为None)")

```

### 2.2 功能详解

导入在mongodb中**不存在**的集合**不保留**原数据

## 3.Import_cover_new_items函数
 
### 3.1 导入

```python
from insert_mongodb import Import_cover_new_items
    #倒库
Import_cover_new_items("数据库","集合名","要导入的文件路径",port=int('数据库端口(默认为27017)'),ip="mongodb数据库所在的ip地址(默认为127.0.0.1)",name="数据库用户名(默认为None)",password="数据库密码(默认为None)")

```

### 3.2 功能详解

导入**全部新的**的集合**不保留**原数据

## 4.append_new_items函数

### 4.1导入
```python
from insert_mongodb import append_new_items
    #倒库
append_new_items("数据库","集合名","要导入的文件路径",port=int('数据库端口(默认为27017)'),ip="mongodb数据库所在的ip地址(默认为127.0.0.1)",name="数据库用户名(默认为None)",password="数据库密码(默认为None)")

```

### 4.2 功能详解


导入**全部新的**的集合**保留**原数据

