# Team Board

## 프로젝트 개요
UX팀(8명) 업무 관리용 칸반 보드. Vercel 호스팅 + Supabase DB + Confluence iframe 임베드.

## 배포
- **URL**: https://team-board-five.vercel.app
- **Vercel 프로젝트명**: team-board

## Supabase
- **Project URL**: https://wfqtukavhmpuymyorznq.supabase.co
- **anon key**: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6IndmcXR1a2F2aG1wdXlteW9yem5xIiwicm9sZSI6ImFub24iLCJpYXQiOjE3NzM5ODIyNTAsImV4cCI6MjA4OTU1ODI1MH0.mR3GrVfmBmxU8rLZ8hCxlEfJYivN-mk9TCAJvzrTdLU
- **테이블**: cards (id, title, description, person, status, start_date, due_date, created_at, position)

## 기술 스택
- 순수 HTML + JS (프레임워크 없음)
- Supabase JS CDN (`@supabase/supabase-js`)
- 드래그앤드롭: HTML5 Drag & Drop API

## 파일 구조
```
team-board/
├── index.html    ← 전체 앱 (HTML + CSS + JS 단일 파일)
├── CLAUDE.md
└── package.json  ← (있다면) Vercel 배포용
```

## 현재 기능
- 칸반 레인 3개: 진행중 / 완료 / 대기
- 카드 추가 (+ 버튼)
- 카드 수정/삭제
- 담당자 필터 (칩 버튼)
- 드래그앤드롭으로 레인 간 이동
- Supabase 실시간 저장
- 월별 기준 관리

## 디자인
- 교육용 템플릿 테마 (크림 배경 #f7f6f3, 카드 흰색, 포인트 #2d5be3)
- Noto Sans KR + JetBrains Mono
- 담당자별 컬러 태그

## Confluence 임베드
- iframe 매크로 사용
- URL: https://team-board-five.vercel.app/
- 높이: 800px 고정
- frameborder: 0

## 남은 작업 / 개선 아이디어
- iframe 외곽 테두리 제거 (Confluence frameborder=0)
- 월 이동 (이전/다음 월) 기능
- 카드 정렬 (드래그 순서 저장)
- 팀원 관리 (추가/삭제)
