# 薪火相承 CRM · 静态高保真原型

Element Plus 风格 PC Web 列表页原型（无后端）。字段与筛选项对齐 `docs/fields-wave1.md`、`docs/fields-wave2.md`；测试数据包含「测试」「测试2026092」。

## 打开方式

### 方式一：直接用浏览器打开（file://）

```bash
# macOS
open /workspace/crm-xinhuo/prototypes/index.html

# Linux
xdg-open /workspace/crm-xinhuo/prototypes/index.html
```

或在资源管理器中双击 `index.html`。

### 方式二：本地静态服务器（推荐）

```bash
cd /workspace/crm-xinhuo/prototypes
python3 -m http.server 8765
```

浏览器访问：http://127.0.0.1:8765/

## 文件结构

```
prototypes/
├── index.html                 # 原型目录（画廊）
├── login.html                 # 登录
├── layout-shell.html          # 布局壳
├── douyin-customer.html       # 抖音 · 客户管理
├── douyin-advertising.html    # 抖音 · 广告账户
├── douyin-consumption.html    # 抖音 · 广告账户消耗
├── douyin-recharge.html       # 抖音 · 账户充值
├── users-role.html            # 人事 · 岗位管理
├── users-user.html            # 人事 · 人事档案
├── contract-contract.html     # 合同管理
├── finance-cashrecharge.html  # 财务 · 现金充值
├── system-menu.html           # 系统 · 菜单管理
├── common-accountopenapply.html # 公共 · 开户申请
├── assets/common.css          # 共享布局样式
└── README.md
```

## 说明

- 相对路径引用 `assets/common.css`，无需构建工具。
- 侧栏菜单、顶栏页签、筛选区、工具栏、表头、分页与现网勘察一致（静态示意，按钮无真实提交）。
- 登录成功链接默认跳转岗位管理（与 PRD 勘察落地页一致）。

## GitHub Pages

一旦启用 Pages（Settings → Pages → Deploy from branch `main` / root），站点地址：

https://jeep91106-cpu.github.io/crm-xinhuo-prototypes/
