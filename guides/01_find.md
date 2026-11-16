---
step: 1
key: find
title: 영상 찾기
ai: false
settings:
  search.keywords: [연애, 남자심리, 여자심리, 썸, 재회]
  search.max_results: 12
  search.rising.min_views: 1000
  search.rising.max_views: 5000
  search.rising.min_views_per_hour: 150
  search.rising.max_hours: 72
  search.rising.allow_post: false
---
# ① 영상 찾기

## 하는 일
키워드로 유튜브를 검색해 **최신 영상**과 **뜨기 직전 영상**을 불러와요. 유튜브는 읽기만 하고, 로그인하지 않아요.

## 기준
- 최신 영상: 키워드 검색 결과를 올린 시각 순으로 `search.max_results`개까지 보여 줘요.
- 뜨기 직전 영상: 조회수가 `min_views`~`max_views`이고, 시간당 조회수가 `min_views_per_hour` 이상이며, 올린 지 `max_hours`시간 안인 영상이에요. 이 영상은 기본으로 **초안까지만** 만들어요(원문 p.4). 설정 '뜨기 직전 영상에도 댓글 달기'를 켜면 댓글도 달 수 있어요.
- 공식 API 키(`YOUTUBE_API_KEY`)가 있으면 공식 API를 쓰고, 없으면 공개 페이지를 읽어요.

## 바꾸는 법
위 `settings` 값을 고치면 다음 [영상 불러오기]부터 반영돼요. 키워드는 1~30개까지 넣을 수 있어요.
