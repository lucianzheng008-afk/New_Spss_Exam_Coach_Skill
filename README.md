# SPSS Exam Coach

Codex skill for SPSS operation exams in Chinese quantitative methods courses. It helps with method choice, SPSS menu paths, output-table reading, direct data calculation, exam-ready conclusions, and textbook/classroom-aligned review for 庞琴《国际关系量化研究方法》.

## Install

This repository uses a flat skill layout: `SKILL.md` is at the repository root. Install it with `$skill-installer` using `--path .` and `--name spss-exam-coach`:

```bash
python /Users/zhengsiyuan/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo lucianzheng008-afk/SPSS_EXAM_COACH_SKILL \
  --path . \
  --name spss-exam-coach
```

Then restart Codex so the skill is discovered.

## Contents

- `SKILL.md`: main routing and response contract.
- `openai.yaml`: Codex UI metadata.
- `spss-operation-map.md`: SPSS menu paths, output names, variable placement, assumptions, templates, and traps.
- `result-interpretation-principles.md`: significance logic, p-value inference, effect-size wording, and automatic result descriptions.
- `data-execution-mode.md`: instructions for computing directly from `.sav`, `.csv`, `.xlsx`, and `.xls` files.
- `textbook-integration.md`: textbook source notes and chapter anchors for 庞琴《国际关系量化研究方法》.
- `textbook-ocr-notes.md`: OCR-confirmed textbook-aligned reminders.
- `classroom-review-v2.md`: uploaded V2 review outline, classroom cases, method distinctions, and exam checklists.
- `spss_exam_analyzer.py`: helper script for auditing and computing common analyses from `.sav`, `.csv`, and Excel files.

## Typical Prompt

```text
Use $spss-exam-coach to analyze this SPSS操作考试题目 or dataset, compute/check the needed statistics, and give the method choice, principle, exact menu steps, output interpretation, inference, and exam-ready conclusion.
```

## Notes

Because this repository is flat, all internal references use root-level filenames, for example:

```text
spss-operation-map.md
data-execution-mode.md
spss_exam_analyzer.py
```

Do not use `references/...`, `scripts/...`, or `spss-exam-coach/...` paths in this flat version.
