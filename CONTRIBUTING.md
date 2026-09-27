# 归档工作流

## 发布版本

- 当前版本：1.0.1
- 发布日期：2026-09-26

### Tag 和 Release 命名

| 类型 | 命名规范 | 示例 |
|------|----------|------|
| Tag | 纯数字版本号 | 0.1.0 |
| Release | v 前缀 | v0.1.0 |

**发布流程**：
1. 创建 tag：`git tag -a 0.1.0 -m "Release 0.1.0"`
2. 推送 tag：`git push origin 0.1.0`
3. 创建 GitHub Release，使用 `v` 前缀

## 归档规则

- 归档来源：清洗后的日记、已完成的项目文档、过期的临时文件
- 归档时机：每周或项目完成后统一归档
- 归档操作：记忆集在归档站有同名一级主题目录（如 `game/`、`fiction/`）时入 `<主题>/journal/`，否则入 `journal/<分类>/`

## 操作步骤

1. 确认源文件已完成清洗
2. 移动文件到 `archive/<主题>/journal/` 或 `archive/journal/<category>/`
3. 提交并推送

## 分类参考

| 分类 | 说明 |
|------|------|
| default | 默认日志 |
| product | 产品相关 |
| write | 写作相关（存量，新 fiction 集日志入 `fiction/journal/`） |
| execute | 执行相关 |
| think | 思考相关 |

一级主题目录（与 `journal/<分类>/` 平级）：

| 目录 | 说明 |
|------|------|
| fiction | 写作主线：作品 + fiction 记忆集日志归档位 |
| game | 游戏主线：项目文档 + game 记忆集日志 |
