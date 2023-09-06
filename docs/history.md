---
hide:
  - navigation
---

## v3.4.7

- `Recorder`对 csv 和 xlsx 文件插入`dict`数据时可自动匹配表头
- `Recorder`增加`set.fit_head()`方法
- `Recorder`和`Filler`的`set.head()`方法增加`table`参数
- `Filler`的`set_link()`可删除已有链接
- 保存失败时会把数据保存到`'failed_data.txt'`文件
- 调整数据处理逻辑
- 修复新版产生的若干问题

---

## v3.4.5

- `Filler`增加`set_img()`方法，可插入图片
- `Filler`增加`set_row_height()`和`set_col_width()`方法
- 修复`Filler`添加单行数据时出现的问题

---

## v3.4.3

- 优化`DBRecorder`写入效率
- `add_data()`增加`table`参数，可为每个数据指定要写入的表
- 处理`'db'`、`'xlxs'`格式时，`data`参数返回值改成`dict`格式
- 坐标增加`'3A'`类型
- `record()`方法出现异常时不再打印数据，也不返回未保存数据

---

## v3.4.2

- `Filler`增加设置单元格样式功能
- 增加`CellStyle`类用于管理单元格样式
- `DBRecorder`增加`run_sql()`方法
- 修改设置项 api，`set_xxxx()`改为`set.xxxx()`形式
- 优化结构和部分逻辑
- 修复`DBRecorder`有关问题

---

## v3.3.2

- `Recorder`支持设置 xlsx 单元格样式，也可跟随原有样式
- 可指定 xlsx 数据表
- 赋值属性增加 set_xxxx() 方法

---

## v3.2.1

- `Filler`可免筛选返回所有行
- `Filler`可免筛选返回所有列
- `Filler`增加`deny_sign`参数，可筛选`sign_col`列值不是`sign`的行
- `Filler`参数顺序有修改
- 修复一些问题
- 写入文件前显示提示语句，避免误关进程导致文件损坏

---

## v3.1.3

- 添加`DBRecorder`
- 可手动指定`type`属性，即无视文件后缀指定记录方式
- 优化`Filler`逻辑

---

## v3.0.0

- `MapGun`功能并入`Filler`，去除`MapGun`
- `ByteRecorder`可指定每条数据在文件中的位置
- `Filler`添加链接时可改变文本颜色
- `record()`保存失败时返回未保存数据
- 优化逻辑，提高可靠性和速度

---

## v2.1.0

- 增加`ByteRecorder`
- 支持灵活的坐标设置
- 优化逻辑

---

## v2.0.1

- 支持多线程同时写入文件

---

## v1.4.0

- `Recorder`支持任意类型
- 记录到txt时不保留list状态

---

## v1.3.0

- `record()`增加`new_path`参数，支持保存到新文件

---

## v1.2.8

- csv 文件也支持`set_link()`

---

## v1.2.7

- 增加`Filler`类和`MapGun`类
- 优化逻辑

---

## V1.0.0

- 基本完成功能
