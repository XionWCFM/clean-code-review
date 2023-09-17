
# 들여쓰기 무시하기

저자는 간단한 if 문, while 문 , 짧은 함수에서

들여쓰기 규칙을 무시하고싶은 유혹이 생긴다고 한다.

나도 실제로 코딩을 할 때 너무 짧은 이프문같은 경우에는

웬만하면 짧게 표현하곤 하는 편이다.

```tsx

const doSomething = (flag:boolean):boolean => {
    if(flag) return true
    return false
}
```

예제가 조금 어색하긴하지만

예를 들면 이런식으로 작성하는 것을 선호한다.

반면 들여쓰기를 넣는다면 어떨까?

```tsx

const doSomething = (flag:boolean):boolean => {
    if(flag) {
        return true
    }
    return false
}
```


오히려 짧은 일을 할 때에는 없는 편이 더 읽기 쉽다고 생각한다.

다만 저자는 나처럼 들여쓰기를 생략하는 방식을 지양한다고 밝힌다.

왜 그런건지 이유를 보니

# 들여쓰기가 있어야 하는 이유

1. 코드에서 각 계층은 블록으로 표현된다.

2. 계층은 즉 선언문과 실행문을 해석하는 범위라고도 볼 수 있다.

3. 프로그래머는 들여쓰기 체계에 크게 의존하며 범위를 시각적으로 인식한다


따라서 범위는 프로그래머가 코드를 읽을 때에 큰 도움을 주기 때문에

이를 어느곳에서든 지켜주는 것이 좋다.

# 내 생각엔

나름대로 일리가 있는 의견이긴하다.

심미적으로 좋은 코드보다 읽기 쉬운 코드를 지향한다면

오히려 이쪽에 더 설득이 되는 것 같다.

한번 도입해보고 괜찮은 것 같으면 유지해볼만 할 것 같다.