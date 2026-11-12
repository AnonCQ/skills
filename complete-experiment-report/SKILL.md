---
name: complete-experiment-report
description: Inspect assignment materials and a project folder, identify every required experiment and deliverable, carry out the experiment, then complete the teacher-provided report template using verified results and relevant visuals. Use for lab reports, course experiments, practical assignments, and related document, screenshot, or presentation deliverables.
---

# Complete Experiment Report

Start from the task folder, determine the full assignment, complete the required experiment and deliverables, and write the report from the supplied template using verified evidence.

## 1. Discover requirements and materials

- Use the folder named by the user. If none is named, use the task's current project folder when it is clear; otherwise ask for the folder.
- Inventory the relevant files before editing or running anything. Inspect assignment instructions, rubrics, teacher templates, existing reports, source code, datasets, screenshots, and prior outputs. Skip unrelated dependency, cache, and build folders unless the task depends on them.
- Determine all explicit deliverables and their required formats, such as a report, source code, data, screenshots, charts, or presentation. Record an internal checklist that maps each requirement to the work and evidence needed; do not create a separate checklist document unless requested.
- Use the available document, spreadsheet, presentation, or other format-specific skill/tool when it materially helps create or inspect a required deliverable.
- Resolve conflicts using the assignment's explicit requirements and the user's latest instructions. Ask only when missing information materially changes the experiment or a required deliverable and cannot be inferred from the materials.

## 2. Design and perform the experiment

- Understand the existing project and experiment objective before changing files. Plan a small, reproducible method that covers each required condition and produces the needed evidence.
- Implement or modify only what the assignment requires. Preserve unrelated project content and existing user work.
- Run the experiment using the available environment. Base results, measurements, tables, conclusions, and visualizations on actual execution and supplied data. Never fabricate successful runs, screenshots, values, or observations.
- Complete every explicitly requested deliverable in its requested format. Create no extra explanatory document or artifact unless the assignment or user requests it.
- If execution is blocked by unavailable hardware, software, access, or input, finish the independent work that remains possible and state the concrete limitation in the final conversation.

## 3. Collect and place visual evidence

- Prefer images naturally exported during execution, such as plots, diagrams, program output images, or saved result charts. Generate charts from real experiment data and keep their source data or generation code when required.
- Use a real application screenshot only when the assignment requires visible UI evidence and no suitable exported image exists. Do not use screenshot placeholders or invented/composited evidence. Do not use Computer Use or UI automation to author documents or collect screenshots.
- Place each figure next to the paragraph or step it supports. Keep explanatory text and its image together; avoid long blocks of prose followed by an unrelated image gallery. Follow the template's figure numbering, caption, and sizing conventions.
- If a required screenshot genuinely needs manual UI capture, do not put a placeholder in the report. Explain the exact reproduction steps and command, when applicable, in the final conversation. Avoid requesting manual screenshots when a genuine exported visual satisfies the requirement.

## 4. Complete the report from its template

Write the report after the experiment results and evidence have been verified.

- On this computer, use the verified LibreOffice command-line executable `D:\LibreOffice\program\soffice.com` (version 26.8.2.2). In PowerShell, invoke it with the call operator `&`. If that path is unavailable in another environment, locate that environment's LibreOffice executable and keep using LibreOffice.
- Prefer LibreOffice for reading, editing, converting, and exporting report documents. Use its headless command line or UNO API where practical; use another direct file/API document tool only when LibreOffice cannot support the required format or preserve the template. Do not use Computer Use for document editing.
- Read the report/template and distinguish completed content from blanks, prompts, `xxx`, examples, and content explicitly required by the assignment.
- Create an untouched backup before modifying the source report or template. Use a clear backup name and do not overwrite an existing backup.
- For a `.docx` report/template, edit that file in place after the backup exists. Fill or replace only missing, placeholder, or explicitly incorrect content. Preserve valid completed content, document structure, styles, page layout, headers, footers, tables, and existing figures.
- For a legacy `.doc` template, preserve the original `.doc` as the backup, convert it to `.docx` with LibreOffice, edit the converted document, and deliver the final report as `.docx`. Prefer headless conversion, for example: `& 'D:\LibreOffice\program\soffice.com' --headless --convert-to docx --outdir "<output-folder>" "<template.doc>"`. Check the converted layout and repair only conversion damage needed to retain the template's intended formatting.
- For other template formats, use an editable, format-preserving workflow appropriate to the format and assignment. Do not recreate the document from scratch when the supplied template can be edited.
- Integrate actual relevant figures into the corresponding report sections. Do not insert screenshot placeholders, and do not append all images after the report narrative.
- Keep the report submission-ready. Do not include assistant commentary, internal analysis, editing steps, or the agent's workflow in the report.

## 5. Verify and deliver

- Confirm each explicit requirement has a corresponding completed artifact or evidence.
- Check that report claims match executed results and source data, required figures appear beside the relevant text, and no placeholder text or fabricated evidence remains.
- Check the report opens and its layout remains consistent with the template, including after `.doc` conversion. Prefer LibreOffice export or other non-UI checks; do not use Computer Use.
- Deliver only the requested artifacts. In the final conversation, list their paths and briefly summarize completion. Give reproduction steps and commands only for genuinely required screenshots the user must capture manually. Do not create a separate explanation or handoff document unless requested.

