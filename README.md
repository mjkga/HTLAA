# How To Learn (ALMOST) Anything

프로그래밍, 디자인, 설계, 임베디드 등 하루 새롭게 시도 또는 배운 것을 다음의 규칙으로 commit한다.
- 참고 : [thoughtbot til 참고](https://github.com/thoughtbot/til)

## Git 명령어 정리

TODO : git commit message 한번에 정리해서 올리기 
'''git 
git log --oneline
git log 
'''
과거 커밋 메시지 여러개 수정하기 
git reabse를 통해서 어느 시점부터 HEAD까지의 커밋을 한번에 rebase한다. 
이미 중앙서버에 push 한 커밋은 절대 고치지 말아야 한다. push한 커밋은 rebase하면 결국 같은 내용을 두번 push하는 것이기 때문이다. 

$ git rebase -i HEAD~3  
멈춘 커밋의 커밋 메시지를 수정할 수 있다.
$ git commit --ammend 

그냥 테스트

## 작성 규칙
- 문서 생성은 
- 언어나 기술명으로 폴더를 만든다. (root에 문서를 만들지 않는다 오직 README.md)
- 파일명은 영어로
- 참고 : JayJin github [Jayjin github](https://github.com/milooy)

