# rank_server

## 数据库中有UserInfo表，包含了客户端号以及分数

## 接口1：http://127.0.0.1:8000/add/client_nums=&score=

### 在接口中包含了client_num（客户端号）与score（分数）客户端的信息，在数据库中查找客户端信息。如果信息不存在则在数据库中新建客户端信息，如果存在更新当前客户端所对应的成绩信息。

## 接口2：http://127.0.0.1:8000/show/client_nums=&low_rank=&high_rank=

### 在接口中包含了client_nums（客户端号）、low_rank（查找起始位置，没有值则默认从第一开始）、high_rank（查找结束位置，没有值则默认到最后一名结束），如果数据库中没有当前查询的客户端信息，则在数据库新建一条信息并且使当前用户的score设置为0
