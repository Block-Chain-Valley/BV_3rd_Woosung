# This file contains memo about questions
- IERC20에는 virtual이 없는데 override가 가능한 이유는?
- Unchecked 키워드를 통해 가스비를 줄이는 건 그렇다치는데, if문으로 오버플로우를 피한다 해도 오버플로우가 나는 상황이면 어떡함? else문 처리법을 모르겠음.
- _spenderAllowance의 주석에 보면 Infinite allowance 방지를 위해 allowance 값을 줄이지 말라 되어있음. 1) infinite allowance가 무엇이며 2)줄여도 되는 게 맞음?
- _msgSender()를 쓰는 이유가 링크에 따르면 "for meta transactions it can be used to return the end user (rather than the relayer)." 라는데 이게 무슨 말임? 1) meta transaction이 무엇인지 2)relayer는 무엇인지 3)그게 왜 문제인지
- Modifier를 다 requirement에 따라 달아주었는데, caller에도 있고 callee에도 있음. 낭비가 아닐까? 원래 이렇게 하는 게 맞음? callee에서 require가 깨졌을 때 caller도 실행이 멈추는지?
- allowance 건드릴 때 먼저 0으로 바꿔둔 뒤 원하는 값을 넣으라고 IERC20 코드 주석에 명시되어있는데 왜 이건 안 함?
