# REVERT 명령어

커밋 되돌리기 ( "git 실습 파일생성")
git revert {커밋 아이디}

편집기(vim)-

(상황1) 기존 메세지 그대로 두고 삭제하는 방법
:(콜론) 키 입력 후, w(write) q(quit)입력
--> 종료

(상황2) 커밋 메세지 직접 수정 하고 저장
i(insert)입력
메시지 수정
esc버튼 입력
-> (콜론) 입력 후, w q 입력
--> 종료

(상황3) 아무것도 하지않고 편집기 강제종료
q! Enter입력
--> revert commit이 생성되지 않고, 그대로 작업 취소

=========================================================
(제미나이의 TIP)
VIM 편집기가 어색하여 사용이 익숙치 않다면 편집기 변경 방법(git bash)
git config --global core.editor "code --wait"
 이거 하고 revert 하면 vscode로 편집기가 작동함 훨씬 직관적이라 편함.

(bash에서 vscode 실행방법)
 code . 하면 vscode가 바로열림