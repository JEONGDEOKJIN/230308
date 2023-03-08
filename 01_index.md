# git 다시 해보기 

1. 새 저장소 만들기 
    git init

2. 터미널 git bash 열기 

3. 파일 스테이징 
`git add .`

4. 커밋 메시지 작성
`git commit -m "메시지 작업 내용"

5. git hub 원격 저장소 연결 
`git remote add origin https://github.com/JEONGDEOKJIN/230308.git`
깃헙에 보면 나옴 

6. push 


# 브런치를 나누기 
- 브런치는 저장소의 작업 공간 
- master 는 최종 작업물, 
- 다른 브런치를 만들어서, 다수가 협업할 때, 혹은 혼자 할 때, 
- 작업 내용을 나눠서 ⭐⭐⭐ -> 최종 작업물로 병합! 
<br>
- 1) master(v0.1) 를 만들어서 작업을 함 -> 2) dev 라는 브랜치를 만듦 -> 계속 dev 에서 작업 -> dev -> 그리고 master(v0.2) 로 병합 
- 왜냐면, master 에는 '완벽한 파일' 만 올리려고 하는 것 ⭐⭐⭐ 

- 마스터에는 '버전' 을 붙인다. ⭐⭐
<br>
- master -> dev1, dev2를 각자 하고 있음 -> dev1 에 병합 (또는 dev2 에 병합) -> master 에 dev1 을 병합. 
<br>
- 작업자 마다 따로 branch 를 파고, dev 작업 하는게 나음. 

<br>

## 브랜치 목록 확인 
- `git branch` 
로컬 저장소의 브랜치 목록 확인
지금은 master 만 있음. 

<br>

- `git branch -a`
원격 저장소와 로컬 저장소 브랜치 목록 확인 

<br>

- 현재 선택되어 있는 branch 는 `* + 초록색 글씨` 로 나옴 

<br>

## 브랜치 생성
- `git branch "생성한 branch 이름"`

<br>

## 생성한 브랜치로 이동 
- `git checkout main`
    - 'main' branch 로 이동하겠다~! 

- `git switch "이동할 브런치 이름"`

## 생성된 브랜치 제거 
- `git branch -d "제거할 브랜치 이름" 
    - 내가 이 브랜치에 있으면 안 지워짐


## 주의사항 
1. 브랜치를 만들었으면, push 를 해서, 원격 저장소에 브랜치를 생성해야 함 ⭐⭐ 

## 저장소 벙합 merge 
- `git merge dev` 
master 로, dev 에서 작업한 걸 가져오기 

- 만약, 충돌이 나면, 파일 보여주고 선택하게 한다. 📛📛📛 
    - 그러면, 변경된거를 push 해줘야 함? 


## 할거 
dev push 하고 
dev 파일 삭제 
작업 공간이 서로 다름 
