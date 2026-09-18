# motion-anything (nexu-io/motion-anything)

## 프로젝트 개요
채팅창에 원하는 연출을 자연어로 적기만 하면 UI 요소나 캐릭터에 자연스럽고 역동적인 움직임을 입혀주는 "대화형 모션 그래픽 레이어"
어려운 키프레임 편집기나 애니메이션 도구 없이도 생동감 넘치는 화면 전환과 인터랙션을 클릭 한 번으로 제작
웹 서비스와 앱 디자인에 프로급 생명력을 불어넣어 사용자들의 시선을 사로잡는 마법의 애니메이션 툴

## 핵심 특징 & 추천 분야
- 대화형모션그래픽
- 자연어애니메이션
- 생동감넘치는UI
- 초간편인터랙션
- 디자인생명력부여

---
*이 문서는 오픈소스 큐레이터(Curator-Agent)에 의해 자동 생성된 가이드 문서입니다.*


---
## 기존 CLAUDE.md 내용

# CLAUDE.md

This project follows a single, tool-agnostic working agreement so it can be continued by any AI
agent in any session.

👉 **Read [`AGENTS.md`](AGENTS.md) first** — it is the source of truth for repo structure,
the recipe manifest schema, the golden path for adding recipes, and the hard rules.

👉 **Then read [`PROGRESS.md`](PROGRESS.md)** — current status and the task queue.

👉 **The motion standard is [`MOTION-SPEC.md`](MOTION-SPEC.md)** — every recipe and the router
skill must obey it.

## Claude-specific notes

- This repo is intentionally plain files (Markdown / YAML / HTML / CSS / JS) with no build step,
  so the user can switch tools or resume in a fresh session at any time without losing context.
  Keep it that way.
- When the user describes a motion in natural language, your job is the loop in
  `skills/motion-anything/SKILL.md`: classify intent → pick recipes from `recipes/` honoring
  `MOTION-SPEC.md` (especially the restraint budget) → produce the output.
- Prefer extending the library and the spec over one-off code. The reusable recipe is the asset.
