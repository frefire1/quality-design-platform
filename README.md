# 通用质量设计平台

面向可靠性工程的全生命周期质量设计桌面工作台。把分析建模、数据映射、项目资料与文件输出集中在一个本地工作台中，支持 macOS 与 Windows。

**当前版本：0.9.0**

## 主要能力

- **分析建模**：故障树 FTA、可靠性框图 RBD、失效模式与影响分析 FMEA/FMECA、事件树 ETA、马尔可夫分析、系统安全性评估 SSA。
- **指标分析**：可靠性预计、维修性预计、测试性建模、保障性与备件规划、威布尔寿命拟合、可靠性增长、可靠性指标分配。
- **FMECA 表头自定义**：可按军用 GJB 1391、民航 FMEA/FMES、民品 FMEA 等预设切换，也可自定义列并绑定计算因子（λ、α、β、t、Cₘ），自动计算危害性。
- **数据导入**：Excel（.xlsx/.xlsm）、CSV、TSV、XML、JSON 的格式识别与字段映射，导入数据可归类为 FMEA 自定义表头。
- **文件导出**：Word、Excel、PDF、CSV；导出内容包含加工后的 RBD 框图模型（SVG/PNG 及结构表）。
- **项目管理**：版本管理、签入签出、零件库、权限控制。
- **联网协作**：通过内网 IP 交换分析项目中的模型、零件和映射模板。
- **账号与授权**：申请—批准—机器码绑定机制；批准码由管理员离线签发，一机一码。

## 下载

| 平台 | 文件 | 说明 |
| --- | --- | --- |
| macOS | `QualityDesignPlatform-0.9.0-macOS.zip` | 通用二进制（Apple Silicon + Intel），已签名 |
| Windows | `QualityDesignPlatform-0.9.0-Windows-x64.zip` | x64 便携版，解压即用 |

下载地址：[GitHub Releases](https://github.com/frefire1/quality-design-platform/releases)

## 安装与使用

### macOS

1. 下载并解压 ZIP，将 `全生命周期质量设计协作工作台.app` 拖入「应用程序」。
2. 首次打开若被 Gatekeeper 拦截，右键选择「打开」，或在「系统设置 → 隐私与安全性」中允许。
3. 注册账号需要管理员签发的批准码，详见 [注册审批流程](docs/注册审批流程说明.md)。

### Windows

1. 下载并解压 ZIP 到任意目录。
2. 运行 `全生命周期质量设计协作工作台.exe`。便携版无需安装。

## 授权说明

软件采用申请—批准—机器码绑定机制。批准码与账号、机器码、申请编号绑定，换账号、换电脑、换申请编号都会失效。账号申请发送至 `frefire1@hotmail.com`，由管理员用专用生成器离线签发批准码后发回。

> 批准码私有密钥由管理员单独保管，**不包含在本仓库及任何发布包中**。请勿将生成器私钥文件随软件分发。

## 目录结构

```
├── README.md                  本说明
├── CHANGELOG.md               版本记录
├── docs/
│   └── 注册审批流程说明.md      注册、登录、密码重置流程
└── releases/                  安装包下载地址与校验值
```

## 技术支持

- 公司网站：https://chengdujiayun.com
- 问题反馈：https://github.com/frefire1/quality-design-platform/issues
