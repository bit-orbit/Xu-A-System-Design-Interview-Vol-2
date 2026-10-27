# AI Agent Guidelines & Technical Translation Standards

This repository contains the Persian conceptual translation and interpretive typesetting of **System Design Interview: An Insider's Guide (Volume 2)** by الکس شو (Alex Xu) و سان لم (Sahn Lam).

---

## 1. Core Translation Directive: Interpretive, Not Literal
**DO NOT TRANSLATE WORD-FOR-WORD OR LITERALLY.**
- Re-explain technical concepts in natural, idiomatic Persian with the conceptual depth of a Senior Software/Systems Engineer.
- Explain *why* architectures and patterns work, detailing trade-offs and real-world production mental models.
- Maintain the original book structure (chapters, sections, sub-sections, diagrams, code blocks, and callouts).

---

## 2. Mandatory Terminology: Developer Persian (DO NOT TRANSLATE LITERALLY)

| English Term | FORBIDDEN (Literal Calque) | MANDATORY (Developer Persian) |
| :--- | :--- | :--- |
| **Scale / Scaling** | مقیاس / مقیاس‌دهی / مقیاس‌پذیری | **اسکیل / اسکیل کردن / اسکیل‌پذیری (Scaling)** |
| **Scale up / Scale down** | افزایش مقیاس / کاهش مقیاس | **اسکیل‌آپ (Scale-up) / اسکیل‌داون (Scale-down)** |
| **Auto-scaling** | مقیاس‌پذیری خودکار | **اسکیل خودکار / Auto-scaling** |
| **Deploy / Deployment** | استقرار دادن | **دیپلوی کردن / دیپلویمنت (Deployment)** |
| **Rollout / Rolling Update**| چرخش / استقرار غلتان | **رولینگ آپدیت (Rolling Update) / انتشار تدریجی** |
| **Rollback** | عقب‌گرد | **رول‌بک (Rollback)** |
| **Pipeline** | خط لوله | **پایپ‌لاین (Pipeline)** |
| **Cache / Caching** | حافظه پنهان | **کش / کش کردن (Cache)** |
| **Trace / Tracing** | ردیابی | **تریس / تریس کردن (Trace / Tracing)** |
| **Queue** | صف | **صف / صف پیام (Queue)** |
| **Worker / Node** | کارگر | **ورکر (Worker) / نود (Node)** |
| **Cluster** | خوشه | **کلاستر (Cluster)** |
| **Namespace** | فضای نام | **نیم‌اسپیس (Namespace)** |
| **Ingress** | ورودی | **اینگرس (Ingress)** |
| **Pod** | پیله | **پاد (Pod)** |

---

## 3. Workflow & Mandatory Review Phase
All work must track against `todo.md`.
- **CRITICAL:** The final phase of any book milestone MUST ALWAYS be the **Review Phase (`فاز بازبینی و تضمین کیفیت نهایی`)**.
- The Review phase requires:
  1. Grep search across `chapters/` for forbidden terms (e.g. `مقیاس`, `استقرار دادن`, `حافظه پنهان`).
  2. Compiling with `typst compile book.typ` with zero errors and zero missing-font warnings.
  3. Validating bilingual terminology in glossary chapter.
