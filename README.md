## Swallow OS

1. 系统底层C基础库使用安卓C库:bionic
2. 系统链接器使用安卓的linker
3. 系统目录层级当使用安卓驱动时直接合并Linux和安卓目录结构
4. 硬件驱动做必要适配层: 安卓驱动、主线Linux驱动
5. 使用systemd的init管理方案
6. 多套用户界面支持: matchbox、早期ubuntu touch unity8、ubports lomiri、postmarketos的多种用户界面 等
7. 先做X11 Server支持,后续补充Wayland Server支持
8. 循序渐进方案实现
9. 定制安卓支持集成可插拔方案


### 阶段一: SurfaceFlinger 主显示服务
1. 使用安卓驱动,适配手机平台
2. X11 Server 作为安卓的Launcher: XSDL XServer
3. 大量重新编译Linux软件
4. 安卓软件管理切换到Linux用户界面中
5. 重要系统应用切换为Linux内软件应用
6. 使用安卓的init管理方案


### 阶段二:  X11 Server 主显示服务
1. 安卓驱动,X11 Server 调用Gralloc、OpenGL ES、Hwcomposer 绘制图形界面
2. 早期 SurfaceFlinger 作为 X11 的应用
3. 后期 安卓应用 桥接为 X11 的应用
4. 安卓应用支持可插拔处理
5. 主线Linux驱动支持
6. 使用systemd的init管理方案


### 致谢

#### Linux & GUN

#### LineageOS
1. https://github.com/LineageOS
2. https://www.lineageos.org

#### libhybris
1. https://github.com/libhybris/libhybris

#### Halium
1. https://halium.org
2. https://github.com/Halium

#### 旗鱼OS
1. https://sailfishos.org
2. https://jolla.com
3. https://sailfishos.club

#### Ubuntu touch
1. https://ubports.com
2. https://forums.ubports.com

#### Droidian
1. https://droidian.org
2. https://github.com/droidian

#### XServer-XSDL
1. https://github.com/pelya/xserver-xsdl

#### OPENTHOS
1. 清华大学参与
2. https://github.com/openthos
3. https://openthos.github.io

#### OpenFDE
1. https://github.com/openfde
2. https://openfde.com
3. https://blog.csdn.net/OpenFDE
