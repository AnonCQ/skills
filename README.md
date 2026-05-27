# Skills

可复用的 Codex skills 集合，用于沉淀常见任务中的稳定工作流与交付规范。

## Available Skills

### complete-experiment-report

用于根据教师提供的模板完成实验报告，重点包括：

- 基于原模板副本填写内容，尽量保留既有排版与格式。
- 报告正文只包含可提交内容，不混入操作说明。
- 对尚未提供的实验截图，使用 `【截图：……】` 形式给出可作为图注的占位说明。
- 同时生成 Markdown 格式的补充说明，列出待补截图、代码位置与提交前检查事项。

目录：[complete-experiment-report](./complete-experiment-report)

## Usage

在 Codex 中调用：

```text
Use $complete-experiment-report to complete my experiment report from the provided template and create a Markdown screenshot checklist.
```

或直接描述需求并指定该 skill，例如：

```text
使用 $complete-experiment-report，根据老师给的实验报告模板完成报告，并生成补充说明 Markdown 文件。
```
