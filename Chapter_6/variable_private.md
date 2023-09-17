# 변수를 비공개로 정의하는 이유

남들이 변수에 의존하지 않게 만들고 싶기 때문이다.

그런데 어째서 많은 프로그래머들이 get, set 함수를 당연하게 public 으로

만들고 비공개해야할 변수를 외부로 노출시키는 것일까?

# 자료 추상화

```java
public class Point {
    public double x
    public double y
}


```

구체적인 포인트 클래스의 예시다.

```java
public interface Point {
    double getX()
    double getY()
    void setCartesion(double x, double y)
    double getR()
    double getTheta()
    void setPolar(double r, double theta)
}

```

반대로 이건 추상적인 포인트 클래스의 예시다.

여기서 놀라운건 추상적인 포인트 클래스가 자료구조를 명백하게 표현하고는 있지만

자료 구조 이상을 표현하고 있다는 것이다.

이 클래스는 조회할때에는 항상 값을 개별적으로 읽어야하지만

값을 설정할 때에는 두 값을 한꺼번에 설정해야만 하도록 코드를 만들었다.

# 얻을 수 있는 교훈

변수 사이에 함수라는 계층을 넣는다고해서 구현이 감추어지는 것이 아니다.

구현을 감추기 위해서는 추상화가 필요하다

그저 get, set 함수를 만드는 것만으로는 구현을 감출 수 없다.

따라서 개발자는 객체가 포함하는 자료를 표현할 가장 좋은 방법을 고민해야한다.

아무 생각없이 get,set 함수를 만들지마라
