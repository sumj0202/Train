# Train
git_advanced 실습 그리고 복습을 위한 reposit 생성
ignore.io 에서 ignore파일을 생성하였음.
ignore 파일에 대한 활용을 계속 실습해 볼 예정임
그리고 이제부터는 visual code를 사용하여 버전 업데이트 예정

push 하면서 생긴 오류
# ! [rejected]        main -> main (non-fast-forward)
-> 로컬 브랜치가 원격 브랜치보다 뒤처져 있다는 의미
즉, 원격 저장소에 새로운 커밋이 추가 됨.
 (원인) GitHub에서 README 수정했었음.
 (해결법) git pull origin main --rebase
    -> 커밋 이력을 깔끔하게 유지하면서 내 커밋을 원격 커밋 뒤에 붙이는 명령어
git push origin main
 << 해결 완료 >>

 (상황2) 혼자 작업하며 강제로 푸시하고 싶음
 git push origin main --force
  이건 좀 주의해야함 .