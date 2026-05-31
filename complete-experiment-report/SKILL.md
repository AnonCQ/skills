---
name: complete-experiment-report
description: Complete course experiment or lab reports from teacher-provided templates by backing up the original file, editing the original report/template in place, preserving already-filled content and required layout, replacing only missing or placeholder content, marking missing screenshots with meaningful Chinese bracket captions, and delivering a separate Markdown completion guide. Use when writing, filling, revising, or finalizing an experiment report, lab report, practical assignment report, or course design report from a DOCX/PDF/other supplied template and project materials.
---

# Complete Experiment Report

## Purpose

Produce a report that the user can submit after adding any unavailable evidence. After creating an untouched backup, edit the original report/template file in place instead of generating a new document. Treat existing filled content and formatting as authoritative unless it is clearly a placeholder that must be replaced. Keep operational guidance out of the report and place it in a separate Markdown guide.

## Required Inputs

Before drafting, locate or request only inputs that materially affect correctness:

- Teacher-provided template and assignment requirements.
- Project/source-code directory, experimental data, commands, and existing result files.
- User identity/course fields required by the template, if not already supplied.
- Desired output location and any naming convention.

Do not invent experimental results, screenshots, measurements, environment versions, conclusions, personal information, or successful execution that is not supported by supplied artifacts.

## Workflow

### 1. Back up, analyze, then edit in place

1. Identify the authoritative teacher-provided template.
2. Create an untouched backup copy before editing, preferably next to the original with a clear suffix such as `-backup` or `-原始备份`.
3. Analyze the document before writing: distinguish content that is already filled correctly from blanks, prompts, `xxx`, sample answers, placeholder images, empty tables, and sections that requirements show must be completed.
4. Edit the original report/template file in place after the backup exists. Do not create a separate completed-report copy unless the user explicitly asks for one.
5. Fill or replace only the areas identified as missing, placeholder, or required-by-assignment. Do not delete, rewrite, reorder, or restyle already-filled content merely to improve it.

Keep the supplied layout intact: cover, headers and footers, page numbering, school/course marks, section ordering, heading styles, fonts, spacing, tables, borders, captions, and required blank fields. Replace placeholders such as `xxx`, prompts, sample paragraphs, blank answer cells, and example text in place, but leave genuine completed content untouched.

If the template format cannot be edited directly, explain the limitation in the Markdown guide and use the closest format-preserving method available.

### 2. Write only submit-ready report content

Fill only the sections or fields that are actually missing or must be replaced under the assignment requirements, such as purpose, environment, principle, procedure, implementation, test data, results, analysis, and summary. Preserve already-filled sections even if they are stylistically imperfect, unless they conflict with the assignment or the user asks for revision.

Write in formal report voice. The report must not contain assistant-to-user commentary such as:

- "请自行修改" or "以下是为你生成的内容".
- Chat-style explanations, workflow notes, confidence disclaimers, or AI references.
- Internal analysis of what was already filled, what needed replacement, or what editing steps were taken.
- Instructions for finding files or taking screenshots, except the formal screenshot caption placeholders defined below.

When evidence is missing, write supported prose only and leave an explicit evidence placeholder rather than fabricating content.

### 3. Add screenshot caption placeholders

Where a required image is not available, insert a visible placeholder in Chinese corner brackets at the intended image position:

```text
【截图：程序运行结果，展示输入数据、输出结果及程序正常结束状态】
```

The bracketed text serves two purposes: it tells the user what image to insert and tells the teacher what the image demonstrates. Therefore:

- Describe the image subject and the key visible evidence, not an internal instruction.
- Keep the wording suitable to remain as an image caption; after an actual image is added, retain or convert it to the template's figure-caption style.
- Use one placeholder per distinct required image and keep it next to the relevant analysis or step.
- Do not claim a screenshot exists when it has not been supplied.
- Avoid exposing credentials, tokens, student private data, or unrelated desktop content; note redaction needs in the Markdown guide, not in report prose.

Good placeholders:

```text
【截图：数据库连接测试结果，展示连接成功提示与目标数据库名称】
【截图：核心功能运行界面，展示新增记录后的列表变化】
【截图：关键算法代码片段，展示排序比较与交换逻辑】
```

Avoid placeholders that do not inform the teacher, such as `【此处放图】` or `【请用户截图】`.

### 4. Cite code and artifacts economically

Include only the code, tables, commands, or results needed to satisfy the report. Do not paste an entire project when a key function or query is enough.

In the report, introduce a code fragment or result as part of the experiment narrative. In the separate guide, identify exactly where the user can locate any required screenshot or excerpt: file path, function/class/section, relevant line range when practical, command to run, and what must be visible.

### 5. Produce two deliverables

Deliver:

1. The completed report based on the teacher template, containing only submission-facing content and any necessary `【截图：...】` caption placeholders.
2. A separate Markdown file named clearly, such as `<报告名称>-补充说明.md`. This is for the user and must not be merged into the submitted report unless the assignment explicitly requests it.

Use this compact structure for the Markdown guide, omitting empty sections:

```markdown
# 实验报告补充说明

## 待补截图

| 报告位置 | 截图内容 | 获取方式或来源 | 注意事项 |
| --- | --- | --- | --- |
| 3.2 功能测试 | 程序运行结果，展示输入与输出 | 运行 `...`；截图窗口结果区域 | 遮挡个人路径 |

## 代码片段定位

| 报告位置 | 文件路径 | 代码位置 | 需展示内容 |
| --- | --- | --- | --- |
| 2.3 核心实现 | `src/...` | `Class.method()` 或行号范围 | 关键处理逻辑 |

## 待确认或待替换内容

- ...

## 提交前检查

- ...
```

Use Markdown for this guide even when the report itself is DOCX, PDF, or another document format.

### 6. Verify before delivery

Check both artifacts before reporting completion:

- The final report still derives from the supplied template and preserves required formatting.
- The untouched backup exists when an editable template was modified.
- The original report/template file, not a regenerated replacement, was edited in place unless the user requested otherwise.
- Already-filled content remains intact except for clearly required replacements.
- Template placeholders, sample answers, and prompt text are either filled or called out in the guide.
- All unavailable screenshots use specific `【截图：...】` captions at the correct positions.
- No user-facing operational explanation, workflow description, or fill-analysis notes appear in the report body.
- Unsupported claims and fabricated evidence are absent.
- The Markdown guide lists remaining screenshot work, code locations, redaction needs, and unresolved fields succinctly.
- Output names and required identity fields conform to the assignment where known.
