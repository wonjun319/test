# 로그 지우기

### (1) 현재 상태를 보존한 새로운 브랜치 만들기
git checkout --orphan clean-branch

### (2) 새로운 브랜치에서 모든 파일 추가
git add -A

### (3) 새로운 커밋 만들기
git commit -m "초기화된 커밋"

### (4) 기존 브랜치를 삭제하고 새 브랜치를 기존 브랜치로 덮어씌우기
git branch -D main
git branch -m main

### (5) 강제 푸시
git push --force origin main


# 익스텐션 백업
code --list-extensions > extensions.txt
<br>
cat extensions.txt |% { code --install-extension $_}
