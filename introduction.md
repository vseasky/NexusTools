# NexusTools

**NexusTools** is a professional multi-protocol communication debugging and data visualization tool for embedded development, IoT, and industrial applications.

## Connectivity

| Type | Description |
|------|-------------|
| Serial | COM port communication |
| USB CDC | Virtual serial port (CDC ACM) |
| USB HID | HID device communication |
| USB WinUSB | WinUSB device communication |
| TCP Server | TCP server, multi-client support |
| TCP Client | TCP client connection |
| UDP | UDP datagram communication |

## Protocol Support

| Protocol | Description |
|----------|-------------|
| NexusProtocol | Native binary protocol with framing and CRC |
| JustFloat | VOFA+ compatible, little-endian float stream |
| FireWater | VOFA+ compatible, CSV text parsing |

## Views

### Transmit View
- Single send with HEX/text mode
- Multi-line send table with per-row channel, enable, period, count
- Periodic send with configurable interval
- Auto-increment counter prefix
- Newline type selection (NULL / LF / CR / CRLF)

### Receive View
- Real-time text display with high-performance large text rendering
- Line-level selection and Ctrl+C copy
- Timestamp display
- Auto-scroll with pause support

### Receive Table View
- Structured packet display with TimeDelta, Time, ID, Direction, Type, Length, Data columns
- Row selection and scrolling
- Frozen header row

### HEX Analyzer
- Hex/ASCII dual-pane display
- Data inspector (uint8/16/32/64, int8/16/32/64, float, double)
- GoTo navigation (offset / line)

### Data Management Panel
- RX/TX channel mapping configuration (cmd, offset, data type)
- GX general variables
- Waveform channel binding (source, expression, color, axis)
- Raw frame inspection
- Configuration save/load (JSON)

### Waveform View (PlotView)
- Multi-channel real-time waveform rendering (up to 64 channels)
- Measurement lines and crosshair cursor
- Per-channel color, visibility, Y-axis binding
- Time axis modes (full timestamp / compact ms)
- Axis lock and auto-fit

### 3D View
- DirectX 11 real-time rendering
- Model import: OBJ, FBX, glTF, GLB, STL, 3DS, DAE (via Assimp)
- JSON scene configuration with node/channel binding
- Camera controls: rotate, zoom, pan
- Lighting and material configuration
- Real-time node value updates from data channels

### Instruments
- **Gauge** — dashboard dial
- **Ruler** — linear scale
- **Thermometer** — temperature display
- **Battery** — charge level
- **Volume** — audio level meter

Each instrument supports channel binding and multiple instances.

## Text Encoding

26 encodings supported for transmit and receive:

UTF-8, GBK, ASCII, Big5, Shift-JIS, ISO-8859-1, GB18030, EUC-KR, UTF-16LE, UTF-16BE, UTF-16, ISO-8859-2, ISO-8859-15, KOI8-R, TIS-620, Windows-1250 ~ 1258, EUC-JP, KOI8-U

## Themes

6 built-in themes: DarkBlue (default), Light, Emerald, Violet, Amber, Rose

## Languages

- English (en-US)
- Simplified Chinese (zh-CN)

## System Requirements

- Windows 10 / 11
- x64 or x86
- DirectX 11 compatible GPU
