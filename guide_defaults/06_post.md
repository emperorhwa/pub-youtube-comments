---
step: 6
key: post
title: 게시
ai: false
settings:
  profile_assign: round_robin
  limits.daily_max_comments: 10
  limits.min_interval_min: 0
  limits.interval_jitter_min: 5
  typing.per_char_ms: [80, 150]
  typing.punct_pause_ms: 300
  posting.timeout_s: 180
---
# ⑥ 게시

## 하는 일
사람이 [댓글 달기]를 누르면, 고른 크롬 프로필로 영상을 열고 댓글 창에 **한 글자씩** 입력한 뒤 [댓글]을 눌러요.
광고 표기는 기본으로 붙이지 않아요(`config.yaml` 의 `posting.disclosure_enabled: true` 로 켜면 내 채널이 아닌 영상에 `[광고] `를 붙여요).

## 기준
- 영상 하나에 댓글 1개, 하루 `daily_max_comments`개까지(전 프로필 합산, 자정 초기화, 안전 상한 20).
- 연속 게시 사이 최소 `min_interval_min`분 + 0~`interval_jitter_min`분. 기본은 0(끔) — 하루 상한만 지켜요. 켜려면 예: 20
- 프로필 배정: `round_robin`(돌아가며 자동) 또는 `manual`(직접 고르기).
- 타이핑: 글자당 `per_char_ms` 범위 + 문장부호 뒤 `punct_pause_ms`. 같은 문장은 늘 같은 리듬이에요(난수 없음).

## 바꾸지 못하는 것
영상당 1개 · 게시마다 사람이 버튼을 누르는 것 · 브라우저 위장 금지.
