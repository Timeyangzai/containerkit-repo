# ContainerKit

Sileo 源：`https://timeyangzai.github.io/containerkit-repo/`

添加后刷新源，搜索并安装或更新 **ContainerKit (all)**；它会为当前架构安装精确匹配的十个基础组件，包括通讯录和运营商组件。

## 2026.11.04.0252 更新

包含容器运行状态、同容器继续使用、历史删除状态收尾，以及按容器硬件信息、定位和剪贴板配置。源码见 [a46a3a3](https://github.com/Timeyangzai/ContainerKit/commit/a46a3a3)；剪贴板 XR 验收见 [记录](https://github.com/Timeyangzai/ContainerKit/blob/main/docs/codex-tasks/pasteboard-per-container-xr-2026-11-04.md)。

- **RootHide**：十个基础组件，Broker 内含 20G75（XR）和 20F75（14 Pro Max）各自匹配的四种系统选装库。选装通过 Manager 的系统层功能开关安装，默认关闭，是否就绪以后台实际回报为准。
- **rootless**：十个基础组件；未完成完整真机验收，本次不附系统选装库。不要把可安装理解为所有系统层功能均已验证。
- 硬件、定位及剪贴板的 App 内功能依赖注入，RootHide 黑名单 App 不生效。剪贴板隔离不覆盖系统 pasted 或直接 IPC，更多边界见项目验收记录。

更新后请在多任务界面完全关闭 ContainerKit 管理器，再重新打开。既有容器和配置保留；所需的越狱依赖由对应环境的软件源提供。
