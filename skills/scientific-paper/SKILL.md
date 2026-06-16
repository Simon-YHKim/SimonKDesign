---
name: scientific-paper
description: >
  Use when the user wants claude scientific — triggers "논문 작성", "LaTeX 수식", "학술 시각화", "peer review", "scientific paper", "latex equations", "academic figures", or /scientific-paper. Produces 학술 논문 작성 — LaTeX 수식, BibTeX 인용, matplotlib/plotly 시각화, peer review 형식 (IEEE/ACM/Nature), arxiv 제출 준비. 차용 출처 slide deck claude-scientific Different from /document-generate (general docs) and /office-docs (Office formats). This is academic-format specific with LaTeX/BibTeX/figure pipelines.
version: 1.0.0
allowed-tools:
  - Bash
  - Read
  - Edit
  - Write
---

# /scientific-paper

학술 논문 작성 — LaTeX 수식, BibTeX 인용, matplotlib/plotly 시각화, peer review 형식 (IEEE/ACM/Nature), arxiv 제출 준비. 차용 출처 slide deck claude-scientific

## When to use

Trigger phrases:
- Korean: 논문 작성, LaTeX 수식, 학술 시각화, peer review
- English: scientific paper, latex equations, academic figures
- Slash: `/scientific-paper`

## What it does

학술 논문 작성 — LaTeX 수식, BibTeX 인용, matplotlib/plotly 시각화, peer review 형식 (IEEE/ACM/Nature), arxiv 제출 준비. 차용 출처 slide deck claude-scientific

## Boundaries

Different from /document-generate (general docs) and /office-docs (Office formats). This is academic-format specific with LaTeX/BibTeX/figure pipelines.

## Operational notes

- 검증 가능 산출물: 사용자가 직접 확인 가능한 파일/URL 우선 생성
- 외부 의존: SKILL body 에 명시 (Vercel CLI, Expo CLI, LaTeX 등)
- 실패 시: 어떤 단계에서 막혔는지 명시, 사용자 결정 받기

## 완료 보고 (HTML) — 표준
작업을 끝내면 **HTML 완료 보고서**를 생성한다 (SimonKCore `completion-report` 표준).
- 첫 화면은 **심플 요약**(한눈 카드 한 줄) + 직관 그래픽/차트(인라인 SVG)·이미지.
- 각 항목 옆 **[자세히] 버튼**(`<details>`)을 펼치면 상세 — 처음부터 쏟지 않는다(progressive disclosure).
- 자체완결 1파일(인라인 CSS/SVG, 무JS) · 사용자 언어 · 현지시간 스탬프.
- Core 있으면 `completion-report` 호출, 없으면 동일 형식으로 인라인 생성.
