# Win Home Assistant

## 说明
这是一个依赖于 Windows 系统的 Hyper-V 的集成 Home Assistant 的镜像文件。
使用时只需打开 Hyper-V，选择导入镜像即可。

## 使用步骤
1. **启用 Hyper-V**  
   请确保您的 Windows 系统已启用 Hyper-V。可以通过以下步骤启用：
    - 打开“控制面板” → “程序和功能” → “启用或关闭 Windows 功能”。
    - 勾选“Hyper-V”，然后点击“确定”。
    - 重启电脑以完成设置。

2. **导入镜像文件**
    - 下载并解压提供的镜像文件。
    - 打开 Hyper-V 管理器，点击右侧的“导入虚拟机”。
    - 浏览到解压后的镜像文件所在路径，按照导入向导完成操作。

3. **启动虚拟机**
    - 在 Hyper-V 管理器中，选择刚刚导入的虚拟机。
    - 点击“启动”，然后双击虚拟机名称进入控制台。

4. **访问 Home Assistant**
    - 启动虚拟机后，在浏览器中访问 `http://<虚拟机IP>:8123`。
    - 按照屏幕指引完成 Home Assistant 的初始配置。

## 问题排查
### 如果无法使用，请参考以下链接自行下载安装：
- [如何在 Windows 上安装 Hyper-V 并运行虚拟机](https://zhuanlan.zhihu.com/p/611203682?utm_psn=1853178213867597824)
- [Home Assistant 安装详细教程](https://zhuanlan.zhihu.com/p/13794650956)

## 注意事项
- 确保您的硬件支持虚拟化技术并已在 BIOS 中启用。
- 运行虚拟机可能会占用较多系统资源，请确保有足够的 CPU 和内存。
- 建议使用较新的 Home Assistant 版本以获得最新功能和安全更新。

## 常见问题
### Q1: 如何找到虚拟机的 IP 地址？
A1: 在虚拟机启动后，可以在控制台中运行 `ipconfig` 获取虚拟机的 IP 地址。

### Q2: 浏览器无法访问 Home Assistant？
A2: 请确保防火墙未阻止端口 8123，或者在虚拟机设置中检查网络适配器是否配置正确。

### Q3: 是否可以在其他系统上使用该镜像？
A3: 目前该镜像仅适用于 Windows Hyper-V 环境。如果需要在其他虚拟化平台（如 VMware 或 VirtualBox）上运行，请自行转换镜像格式。

---

## 更新与反馈
如果在使用过程中遇到任何问题或有改进建议，请通过以下方式联系我们：
- **邮箱**: support@example.com
- **GitHub**: [项目主页](https://github.com/example/win-home-assistant)

欢迎提交反馈与建议，我们将持续优化镜像体验。

