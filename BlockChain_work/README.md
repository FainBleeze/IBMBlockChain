# IBMBlockChain
IBM 区块链后端实现。定义了基本的业务模型和事务执行逻辑代码。

### 模型部分(.cto文件)

##### 定义了Asset类

- Order（订单ID，商家，买家，商品信息，订单状态）

##### 定义了三个Participant类

- 虚类Account（用户ID，用户资金，信息记录）
- seller类，在继承account的基础上添加了商品列表和订单列表
- buyer类，在继承account的基础上添加了订单列表

##### 定义了六个业务，并在js中予以实现

- 商家相关的业务：
  + 增加商品
  + 下架商品
  + 确认发货
- 买家相关的业务：
  + 建立订单
  + 取消订单
  + 确认收货
