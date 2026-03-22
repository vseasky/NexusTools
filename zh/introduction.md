# NexusTools

**NexusTools** 是一款专业的多协议通信调试与数据可视化工具，面向嵌入式开发、物联网及工业应用场景。

## 连接方式

| 类型 | 说明 |
|------|------|
| Serial | COM 串口通信 |
| USB CDC | 虚拟串口 (CDC ACM) |
| USB HID | HID 设备通信 |
| USB WinUSB | WinUSB 设备通信 |
| TCP Server | TCP 服务端，支持多客户端 |
| TCP Client | TCP 客户端连接 |
| UDP | UDP 数据报通信 |

## 协议支持

| 协议 | 说明 |
|------|------|
| NexusProtocol | 原生二进制协议，帧结构 + CRC 校验 |
| JustFloat | VOFA+ 兼容，小端浮点字节流 |
| FireWater | VOFA+ 兼容，CSV 文本解析 |

## 功能视图

### 发送视图
- 单条发送，支持 HEX / 文本模式
- 多条发送表格，每行独立配置通道、使能、周期、次数
- 周期发送，可配置发送间隔
- 自增计数前缀
- 换行类型选择 (NULL / LF / CR / CRLF)

### 接收视图
- 实时文本显示，高性能大文本渲染
- 行级选中与 Ctrl+C 复制
- 时间戳显示
- 自动滚动与暂停

### 接收表格视图
- 结构化数据包显示：TimeDelta、Time、ID、Direction、Type、Length、Data
- 行选中与滚动
- 冻结表头行

### HEX 分析器
- 十六进制 / ASCII 双面板显示
- 数据检查器 (uint8/16/32/64, int8/16/32/64, float, double)
- GoTo 导航 (偏移 / 行)

### 数据管理面板
- RX/TX 通道映射配置 (cmd, offset, 数据类型)
- GX 通用变量
- 波形通道绑定 (来源、表达式、颜色、坐标轴)
- 原始帧查看
- 配置保存/加载 (JSON)

### 波形视图 (PlotView)
- 多通道实时波形渲染 (最多 64 通道)
- 测量线与十字光标
- 每通道颜色、可见性、Y 轴绑定
- 时间轴模式 (完整时间戳 / 精简毫秒)
- 坐标轴锁定与自适应

### 3D 视图
- DirectX 11 实时渲染
- 模型导入：OBJ, FBX, glTF, GLB, STL, 3DS, DAE (Assimp)
- JSON 场景配置，节点/通道绑定
- 相机控制：旋转、缩放、平移
- 光照与材质配置
- 实时数据通道驱动节点更新

### 仪表控件
- **仪表盘** — 圆盘仪表
- **标尺** — 线性刻度
- **温度计** — 温度显示
- **电池** — 电量指示
- **音量计** — 音量电平

每种仪表支持通道绑定，可创建多个实例。

## 文本编码

支持 26 种编码格式：

UTF-8, GBK, ASCII, Big5, Shift-JIS, ISO-8859-1, GB18030, EUC-KR, UTF-16LE, UTF-16BE, UTF-16, ISO-8859-2, ISO-8859-15, KOI8-R, TIS-620, Windows-1250 ~ 1258, EUC-JP, KOI8-U

## 主题

6 套内置主题：DarkBlue (默认), Light, Emerald, Violet, Amber, Rose

## 语言

- English (en-US)
- 简体中文 (zh-CN)

## 系统要求

- Windows 10 / 11
- x64 或 x86 架构
- 支持 DirectX 11 的显卡
