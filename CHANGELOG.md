# 更新日志

## 4.2.11 - 2024/12/01

- 阿里云 Maven 仓库问题。
- FIX #90 预取标识符回调问题。

## 4.2.10 - 2024/10/15

- GMS获取ADID时优化，感谢 @a365344743s 贡献。
- 更新奇酷手机混淆规则

## 4.2.9 - 2024/03/07

- 支持360OS手机OAID，感谢 @10cl 贡献。
- 荣耀真机验证荣耀广告标识符SDK。
- 商用法律风险声明。

## 4.2.8 - 2023/12/05

- 支持通过荣耀官方广告标识服务SDK获取OAID [Issues#73](https://github.com/gzu-liyujiang/Android_CN_OAID/issues/73)；

## 4.2.7 - 2023/11/12

- 修复华为高版本手机可能的闪退或卡死问题： [Issues#63](https://github.com/gzu-liyujiang/Android_CN_OAID/issues/63) [Issues#72](https://github.com/gzu-liyujiang/Android_CN_OAID/issues/72)。
- 增加一些文档注释及一些易用的方法。
- 更新演示的安装包到v4.2.7。

## 4.2.6.2 - 2023/11/02

- 更新演示的安装包到v4.2.6。
- 更新 JavaDoc 到 4.2.6。

## 4.2.6 - 2023/11/01

- PR#70 支持老版的OPPO手机获取OAID，感谢@luoyesiqiu的贡献。
- PR#71 通过注册方式预取OAID开放回调接口，感谢@Mankin的参与。

## 4.2.5.1 - 2023/07/17

- 华为手机OAID获取适配，参阅 [Issues#66](https://github.com/gzu-liyujiang/Android_CN_OAID/issues/66) 。

## 4.2.4 - 2022/02/10

- OAID初始化获取为空后需再次获取，避免一直为空。

## 4.2.3 - 2021/09/01

- 新增`DeviceIdentifier`代替`DeviceID`，用于解决APP合规性检测机构检测到的频繁读取设备信息问题；
- 适配 Android 11+；

## 4.2.2 - 2021/08/26

- 增加对酷派（CoolOS）、酷赛（Prize）、卓易（Freeme）的支持，参阅 [Issues#31](https://github.com/gzu-liyujiang/Android_CN_OAID/issues/31) ；
- 提取备份 [手机厂商开放匿名设备标识符获取接口(AIDL)](https://github.com/gzu-liyujiang/Android_CN_OAID/tree/master/aidl) ；

## 4.2.1 - 2021/06/30

- [issues#30](https://github.com/gzu-liyujiang/Android_CN_OAID/issues/30) NoSuchMethodError: No  virtual method getMeid()；

## 4.2.0 - 2021/06/29

- 移除 AndroidX annotation 库的依赖以便兼容 Support v4/v7 项目，参阅 [note_5547665](https://gitee.com/li_yu_jiang/Android_CN_OAID#note_5547665)；

## 4.1.4 - 2021/06/16

- 去除 `WRITE_EXTERNAL_STORAGE` 等相关权限的最大 SDK 限制，参阅 [Issues#25](https://github.com/gzu-liyujiang/Android_CN_OAID/issues/25)；

## 4.1.3 - 2021/05/21

- 代码质量提升（Powered by Gitee Scan）

## 4.1.2 - 2021/05/20

- 精简代码，优化打印调试日志。
- 修复 Android 6.0 以下系统版本获取 GUID 闪退（NoSuchMethodError: No static method canWrite...）。
- 改进 Android 6.0 以下系统版本 GUID 持久化、稳定性。

## 4.1.1 - 2021/05/15

- 加入 `READ_PHONE_STATE`及`WRITE_EXTERNAL_STORAGE` 权限以便适配低版本安卓系统。

## 4.1.0 - 2021/05/14

- 支持中兴及 Motorola、HTC、LG、Sony 等海外平台手机获取 AAID（安卓广告标识符）。
- 华为 OAID 获取优化，支持大屏电视。
- 修复努比亚支持情况识别。
- 处理用户关闭了广告标识符的情况。
- 通过云真机在线调试，更新更多真机实测效果图。

## 4.0.1 - 2021/05/13

- 修复联想、中兴、华硕等 OAID 获取。
- 增加更多品牌真机实测效果图。

## 4.0.0 - 2021/04/29

- **重新打造与移动安全联盟 SDK 的共存方案**，避免因此造成`Issues#22`之类的问题。
- 增强 GUID 在 Android 10 以下版本系统的上的稳定性。
- 避免可能会意外发生的未知异常（`Issues#21`、`PR#23`）。

## 3.0.3 - 2021/04/14

- 更细致的识别手机厂商及其品牌，增加荣耀、红米、爱酷、真我等品牌的支持。

## 3.0.2 - 2021/04/08

- 小米手机获取 OAID 问题（`PR#18`）。
- 增加数字版权管理设备 ID （注：根据`semver.org`语义化版本规范，此处做了向下兼容的功能性新增，版本号其实应该定为`3.1.0`）。
- 增加各大手机厂商关于 OAID 的说明文档。
- 允许判断设备是否支持 OAID（`PR#19`）。

## 3.0.1 - 2021/03/29

- 增加设备标识符统一格式为 MD5 或 SHA1 的方法

## 3.0.0 - 2021/03/26

- 移除之前版本已废弃的方法，重构部分 API。
- 支持在应用启动时预先获取设备的客户端标识。
- 增加 JavaDoc ，更新说明文档。
- 移除 Github Actions 的 CodeQL。

## 2.1.1 - 2021/03/03

- 修复魅族手机获取 OAID 失败问题，增加魅族效果图。

## 2.1.0 - 2021/01/19

- 增加 IMEI/MEID、AndroidID、GUID 等获取方法。
- 优化文档及调整其他一些细节。

## 2.0.0 - 2021/01/13

- 修复 Demo 编译错误（`Isuues#8`）。
- 分包，解决和移动安全联盟 SDK 冲突问题。
- 引入华为云真机调试方案。
- 修正文档错误。
- 修复 Github Actions 错误。

## 1.0.2 - 2020/08/20

- 规避可能的闪退。
- 使用 Github Actions 代替 Travis-CI。
- 更新说明文档。

## 1.0.1 - 2020/07/15

- 取消不支持 OAID 时默认生成的 GUID。

## 1.0.0 - 2020/05/30

- 初始版本。
