---
step: 4
key: comment
title: 댓글 작성
ai: true
settings:
  comment.min_chars: 40
  comment.max_chars: 120
  ai.max_attempts: 3
  comment.candidates: 3
  ai.parallel: 3
---
# ④ 댓글 작성

## 하는 일
AI가 고민에 공감하는 댓글 초안을 써요. 영상 속 장면이나 말을 하나 이상 짚고, 운명원을 '남에게 들은 이야기 + 나도 궁금함' 수위로 한 번 언급해요.
영상마다 시작 방식과 운명원 언급 방식이 달라요(영상 ID로 정해서, 같은 영상은 늘 같은 방식).

## AI 지침
- 영상 속 전문 용어는 영상을 안 본 사람도 알게 풀어 쓴다.
- 편한 구어체로 쓴다(말줄임표·이모티콘은 없어도 된다). 줄바꿈 없이 한 단락으로 쓴다.

## 바꾸는 법
- `comment.min_chars` · `comment.max_chars`: 글자 수. 원문 기준은 40~120자예요.
- `ai.max_attempts`: 규칙에 안 맞을 때 AI가 다시 쓰는 최대 횟수(1~5).
- 위 'AI 지침'의 줄을 고치거나 더하면, 다음 초안부터 AI에게 그대로 전달돼요.
