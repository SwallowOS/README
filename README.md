## Swallow OS
### 中文名为： 燕子系统
### 不同方案系统发布名称都叫:Swallow OS

1. 系统底层C基础库使用安卓C库:bionic
2. 系统链接器使用安卓的linker
3. 系统目录层级当使用安卓驱动时直接合并Linux和安卓目录结构
4. 硬件驱动做必要适配层: 安卓驱动、标准的Linux驱动
5. 使用systemd的init方案
6. 安卓和Linux互为子系统方案
7. 多套用户界面支持: matchbox、早期ubuntu touch unity8、ubports lomiri 等
8. 先做X11 Server支持,后续补充Wayland Server支持

### 方案一: Linux为主系统
1. 标准Linux驱动 
2. 安卓驱动
3. 早期 SurfaceFlinger 作为 X11 的应用
4. 后期 安卓应用 桥接为 X11 的应用

### 方案二: 安卓为主系统
1. 早期 X11 Server 作为 SurfaceFlinger 的应用
2. 后期 X11 应用桥接为 SurfaceFlinger 的应用

### 方案三: 互为子系统
1. 适配层可切换方案