# boundary

시스템에 들어가는 모든 소프트웨어를 직접 개발하는 경우는 드뭅니다.

때로는 패키지를 떄로는 오픈소스를 사용하는데요

요즘 가장 많이 고민하는 부분이기도 합니다.

주로 개발생산성을 위해 프레임워크를 선택하게되는데요

이렇게 개발해둔 프로젝트들을 테스트하려고보면

내 코드들이 프레임워크에 종속되어 프레임워크가 없으면 동작하지 않는다는 사실을 깨닫게 되어서 그런것 같습니다.


이 8장에서는 소프트웨어의 경계를 깔끔하게 처리하는 기법을 설명해준다고 해서 기대가되네요

# 외부 코드 사용하기

인터페이스 제공자와 사용자 사이에는 긴장이 존재한다고 합니다.

프레임워크 제공자는 최대한 범용적으로 사용할 수 있게 애쓰지만

사용자는 자신의 요구사항에 맞는 인터페이스를 바라니까요


# 학습 테스트하기

외부 코드를 통합하는 것은 어렵습니다.

게다가 외부코드를 우리 코드와 같이 동작하게 하는 건 두배로 어렵죠

그러니 우리쪽 코드를 작성해서 외부 코드를 호출하는 것 대신에

테스트 코드를 작성하는 걸 통해 외부 코드를 학습하면 어떨까요?

이런것을 학습 테스트라고 부릅니다.

이런 학습 테스트는 새 라이브러리를 도입하는 것 뿐만 아니라

기존 라이브러리의 메이저 버전 등을 올릴때에도 유용한데요

사실 저도 리액트쿼리 5버전으로 올리기 무서워서 4버전을 쓰고싶은 유혹이 있었는데

이런 경우에도 유용할 듯 합니다.

# 클린한 경계

경계에서는 흥미로운일이 많이 벌어지는데요

소프트웨어 설계가 우수하다면 변경에 많은 투자와 재작업이 필요하지 않습니다.

또한 코드는 통제불가능한 외부패키지에 의존하는것보다

통제 가능한 우리 코드에 의존하는 편이 훨씬 좋으며

외부패키지를 호출하는 코드를 가능한 줄여 경계를 관리하는 것이 좋습니다.


예를 들면 새로운 클래스로 경계를 감싸거나 어댑터 패턴을 사용해

우리가 원하는 인터페이스를 패키지가 제공하는 인터페이스로 변환합시다.

