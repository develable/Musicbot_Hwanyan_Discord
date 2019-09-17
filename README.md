# About Us

Develable

Whatever you imagine, We develop.

상상하는 모든 것을 개발합니다.

# About Project

"누구나 간단하게 운영할 수 있는 음악봇을 만들어 보자!"라는 취지에서 시작되었습니다.

'Project Hwanyan'은 일반인도 쉽게 뮤직봇을 만들고 사용할 수 있도록, 모든 명령어를 한국어로 했으며, 가이드도 제공되어 있습니다.

# About Us

Develable

청소년들의 디스코드 채팅봇 개발 프로젝트

그 중에서도 화냥봇이 두번째 프로젝트입니다.

기획 - [화향](https://hwahyang.space)

개발자 - [엔돔](http://endom.kro.kr)

# Contact

[Develable 공식 홈페이지](https://develable.xyz)

[Develable 지원서버](https://invite.gg/Develable)

[담당자 엔돔 이메일](mailto:dyyeom1@naver.com)

[담당자 화향 이메일](mailto:hwahyang@develable.xyz)

# How to Invite

화냥봇은 저희가 서비스 하는 봇이 아닌, 여러분이 직접 구동하셔서 쓸수 있도록 **소스만 배포하고 있습니다**.

# Self-Hosting

## 안내

~~메인 개발자이신 [엔돔](http://endom.kro.kr)님과 협의하에 더 이상의 지원을 중단합니다.
깃허브에서는 계속 코드를 공개하지만, **코드에 대한 지원은 더 이상 진행하지 않으니** 참고해 주시기 바랍니다.~~

~~안녕하세요? 개발자 엔돔입니다. 화냥봇에 대한 공식적인 지원은 중단한다고 하였지만, 왜인지 모르게 저는 여기에 집착이 남는군요.
하지만 요즘 학업도 그렇고, 여러 사정이 겹치고 시간도 없다 보니 뭐 올해 안에 다시 시작하기는 글렀네요.
개인 포트폴리오로 시작한 Project DW가 벌써 개발을 시작한지 반 년이 다되가네요..
근데 뭐 그렇다 할만한 기록은 안 나오고 있으니 뭐 덜떠름 할 뿐이지요.
그리고 지금 DW도 두 번이나 갈아엎고, 개발하기도 힘든 상황입니다. 그래서 잠시 쉬다시피 다시 화냥봇에 머물러 보려 합니다.
여름방학시즌 전까지로 예상되며, 그 기간 안에는 DW는 잠시 손 놓고, 화냥봇에 대한 지원을 해드리려 합니다.
뭐 업데이트라던가 버그 수정이라던가 그런 건 아니고, 화냥봇으로 봇을 구축해보시는, 음악봇 구축을 연습해보시는 분들에 대한 지원을 해드리려 합니다.
봇을 구축하다가, 어려운 점에 놓이면 언제든지 불러주세요. 저도 현타를 맞고선 지금 DW는 거의 손 놓은 상태라서 짬나는 시간에 하던 개발도 힘들어졌어요.
당분간 화냥봇에 대한 궁금증, 문의, 질문은 적극적으로 답변해드릴게요...
그리고 Dw JS는 당분간 커밋이 없을 예정이에요...~~

현재 화냥봇의 개선 버전인 새로운 음악봇을 개발중에 있으며, 정확한 공개 일정은 정해지지 않았습니다.
현재도 공식서버에서 화냥봇에 대한 지원, 질문 등을 받고 있습니다! 

## 화냥봇 설치 - 기본 구축

구축은 Windows 10 기준입니다.
http://nodejs.org 에서 Node.js를 설치해줍니다.
https://ffmpeg.zeranoe.com/builds/ 에서 ffmpeg의 빌드를 다운받아 C드라이브에 압축해제 해줍니다.
Win + X를 누른 후, 시스템 -> 시스템 정보 -> 고급 시스템 설정 -> 환경 변수 순으로 들어가서
Path에 압축을 푼 ffmpeg의 bin폴더를 추가합니다
ex) 내가 만약 C:\ffmpeg로 풀었다면, Path에 C:\ffmpeg\bin을 추가.
봇의 구축 방법은 알고있다 치겠습니다. 
만약 모르신다면, 유튜브에 있는 다른 강의들을 보시면 꼭 자바스크립트가 아니더라도 봇 계정을 생성하고 연동하는 부분이 있습니다.
그 부분을 이해하신다면 충분히 여기에 적용 가능합니다.
추가하고 나서, 프로젝트 폴더를 만들어줍니다.

## 화냥봇 설치 - 소스코드 다운로드

프로젝트 폴더를 파일 탐색기로 연 상태에서, 파일탐색기의 텅 빈 하얀 부분을 Ctrl + Shift + 우클릭 합니다.
여기에 PowerShell창 열기를 누른 후, `npm i hwanyang` 이라고 치면 많은 파일들이 설치됩니다.
잠시 기다린 후에, 설치가 완료되었다면 PowerShell을 끄셔도 좋습니다.
추가된 `node_modules`라는 폴더로 들어가서, `hwanyang`폴더를 찾습니다.
이제부터 거기가 우리 화냥이의 소스코드가 있는 장소입니다.

- 개발 중단으로 인하여 위의 방법이 유효하지 않을 수 있습니다. **그럴 경우, `branch`에서 `old`를 찾아서 다운받으세요**.

## 화냥봇 구동

아주 간단합니다. 어떤 에디터로든 `settings.json`을 열어줍니다. (Visual Studio Code를 권장합니다)
열고 나서, `Token`에는 봇의 토큰을, `prefix`에는 봇의 접두사(기본은 `냥아`입니다.)를 적어줍니다.
저장 후, `run.bat`을 실행 후, **화냥봇 구동 완료!** 라는 메세지가 뜨면 구동에 성공한 것입니다.
만약 구동이 안되었다면, 자세한 내용을 Develable 공식 디스코드에 문의해주시기 바랍니다.

# 저작권 고지

화냥봇 소스에 대한 저작권은 Develable에서 소유합니다. 모든 권리를 보유합니다.

# 라이선스 고지

[`old` branch](https://github.com/develable/Musicbot_Hwanyan_Discord/blob/old/LICENSE)를 참고하세요
