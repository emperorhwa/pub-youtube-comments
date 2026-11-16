---
step: 5
key: check
title: 규칙 검사
ai: false
settings:
  checks.banned_words: []
  checks.fake_review_words: []
  checks.evidence_min_chars: 6
---
# ⑤ 규칙 검사

## 하는 일
게시 전에 8가지를 **모두** 통과해야 [댓글 달기]가 열려요. 사람이 고친 문장도 다시 검사해요.

| 검사 | 기준 |
|---|---|
| 글자 수 | 40~120자 |
| 운명원 | 정확히 1번 |
| 링크 · 해시태그 | 없어야 함 |
| 지어낸 후기 | '받아봤는데' · '후기' 같은 이용 경험 표현 없음 |
| 금지어 | 욕설 · 비하 · 과장 단정 없음 (+ 아래 `banned_words`) |
| 다른 영상과 다름 | 앞서 쓴 댓글과 겹치지 않음 |
| 장면 인용 | 영상 속 말을 `evidence_min_chars`자 이상 그대로 짚음 |

## 바꾸는 법
- `checks.banned_words`: 기본 금지어에 **더할** 말 목록. 예: `[대박, 존맛]`
- `checks.fake_review_words`: '지어낸 후기'로 볼 표현을 더해요.
- `checks.evidence_min_chars`: 장면 인용으로 인정할 최소 글자 수(4~20).
- 기본 규칙(링크 · 해시태그 · 운명원 1번)은 원문 필수라 이 파일로 끌 수 없어요.
