# 班级活动报名与统计网页

这是第15周课堂使用的 Flask 动态网页协作案例。

## 本地运行

在 Windows PowerShell 中进入项目根目录后执行：

```powershell
python -m venv .venv
.\.venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

如果 `python` 不可用，改用：

```powershell
py -m venv .venv
.\.venv\Scripts\activate
pip install -r requirements.txt
py app.py
```

打开浏览器访问：

```text
http://127.0.0.1:5000
```

## 五人协作分工

| 角色 | 分支名 | 修改文件 | 网页可见效果 |
|---|---|---|---|
| 组长 | main | README.md、Vercel 设置 | GitHub 仓库和线上网址 |
| 组员 A | member-a-event-info | data/event_info.py | 首页标题、活动说明、协作提示变化 |
| 组员 B | member-b-options | data/options.py | 小组选项和活动方向变化 |
| 组员 C | member-c-page-text | data/page_text.py | 表单提示和结果页标题变化 |
| 组员 D | member-d-sample-data | data/registrations.py | 默认报名记录、统计人数和列表变化 |
| 组员 E | member-e-readme | README.md | 汇总所有组员贡献并完善文档 |

## 各组员具体贡献

### 组员 A - 活动基本信息
修改文件：`data/event_info.py`
- 活动名称：班级活动报名与统计网页
- 活动说明：用 Flask 做一个可以填写表单、提交报名、查看统计结果的动态网页
- 协作提示：本项目由 5 人小组通过 GitHub Issue、Fork、Pull Request 和 Review 协作完成

### 组员 B - 小组和活动方向选项
修改文件：`data/options.py`
- 小组选项：第 1 组 ~ 第 5 组
- 活动方向：Python 网页开发体验、校园生活建议收集、AI 工具使用分享、期末项目展示准备

### 组员 C - 页面提示文案
修改文件：`data/page_text.py`
- 首页欢迎语：请填写报名信息，提交后可以看到全班报名统计结果
- 表单填写提示：姓名、小组和活动方向是必填项；一句话说明可以写你为什么想参加
- 结果页标题：报名统计结果

### 组员 D - 默认报名数据
修改文件：`data/registrations.py`
- 示例记录 1：示例同学 A（第 1 组，Python 网页开发体验）
- 示例记录 2：示例同学 B（第 2 组，AI 工具使用分享）

## Vercel 部署

仓库合并完成后，组长在 Vercel 导入 GitHub 仓库。项目根目录保持默认，框架选择 Other，部署完成后访问 Vercel 提供的网址。
