# what is bad code

나쁜 코드란 무엇일까? 좋은 코드는 무엇일까?

굉장히 추상적인 개념이기 때문에

공공연히 좋은 코드를 지향한다고 떠들고 다니는 나의 입장에서는

꽤 많이 답변하게 된 질문이기도 하다.

여러가지 정의가 있을 수 있지만 내가 생각하는 나쁜 코드는

변경을 어렵게 하고 흐름을 예측하기 어렵게 하는 코드라고 생각한다.

그리고 대부분의 코딩 방법론들은 더욱 큰 개념들을 포용하거나 생각하기도 하지만

작은 관점에서는 결국 개발자가 코드와 동작을 이해하기 쉽게 하고

코드를 변경하기 쉬운 구조로 만들고자 하는 데에 가치가 있다고 생각한다.


# 코드 퀄리티와 시간의 trade off

저자는 빨리 가기 위해 나쁜 코드를 쓰지 않아야한다고 말한다.

이는 전적으로 맞는 말이다.

나쁜 코드는 재앙을 불러온다. 그건 모두가 알고 있다.

그러나 현실적으로 좋은 코드를 쓰기 위해서는

나쁜 코드를 쓰는 것보다 고민할 것도 많아지고 생각도 많아지게 되며

이는 단기적인 관점에서 개발 속도의 저하를 만든다.


<br/>

우리는 코딩할 때 새로운 코드를 쓰는 것보다 읽는 시간이 훨씬 길다.

그리고 내가 작성한 코드도 미래의 나는 마치 타인이 작성한 것처럼 느낄 것이다.

그래서 나는 좋은 코드가 불러오는 생산성을 잘 체감하곤 했다.

잘 정리된 코드와 구조는 내가 어떤 기능을 추가할 때에도

쉽게 그것을 허용해주었다.


# what is clean - code?


```
나는 우아하고 효율적인 코드를 좋아한다.

논리가 간단해야 버그가 숨어들지 못한다.

의존성을 최대한 줄여야 유지보수가 쉬워진다.

깨끗한 코드는 한 가지를 제대로 한다.

```

```
깨끗한 코드는 단순하고 직접적이다.

깨끗한 코드는 잘 쓴 문장처럼 읽힌다.

깨끗한 코드는 결코 설계자의 의도를 숨기지 않는다.

오히려 명쾌한 추상화와 단순한 제어문으로 가득하다.
```

책에서 인용한 문장을 인용했다.

인용의 인용.. 이긴 한데 결국 나는 클린코드의 시작이

관심사의 분리로부터 시작한다는 생각을 했다.

함수가 하나의 일을 잘하도록 역할을 분리하면

그만큼 버그가 발생할 여지가 줄어들고 함수의 동작을 쉽게 예상할 수 있다.

그리고 그렇게 쪼개둔 함수는 내가 에상치 못한 곳에서 재활용되곤 한다.

그래서 나는 역할을 잘게 쪼개는 것을 선호하는 편이다.

그것이 내가 생각하는 깨끗한 코드이기 때문이다

# 마치며

처음부터 정리하면서 적을걸 그랬습니다.

그래도 다시 읽어보니 또 새롭네요
