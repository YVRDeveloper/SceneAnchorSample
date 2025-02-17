# 焦点感知

焦点感知功能允许系统 UI 作为应用场景顶部的覆盖显示。因此，用户访问系统 UI 时无需退出当前应用，保证用户获得不间断的沉浸式 VR 体验。
注意事项


## 注意事项

- 焦点感知功能仅提供事件，不提供接口
- 若不适配此功能，点击手柄 Home 键时，可能会出现2幅手柄模型重叠的情况。


## 事件说明

焦点感知相关事件如下：

| **事件** | **说明** | 
| ------- | -------- |
| YVRManager.instance.eventsManager.onFocusGained | 应用程序失去输入焦点。例如：应用程序运行时，若用户按下手柄上的 Home 按钮，系统 UI 显示，应用程序会失去输入焦点。此时，开发者可以暂停游戏、禁用用户的输入功能（例如手柄）或通知其他在线用户该用户当前没有专注于应用程序。 | 
| YVRManager.instance.eventsManager.onFocusLost | 应用程序获得输入焦点。系统 UI 被关闭时，该事件触发。此时，开发者可以恢复游戏或开启用户的输入功能。 | 