# -
문제상황은 이러하다. python에서 id()라는 함수를 통해 object의 메모리주소값을 확인 할 수 있는데 -5~256까지의 값은 모두 같은 메모리값을 가지는 반면

그 이외의 값을 모두 다른 메모리값을 갖는데 그 이유에 대해서 알아야하는 문제였다.

제출하기 위해서는 증명을 위한 코드?와 설명을 포함해야하는데 증명을 위한 코드를 무엇을 써야하는지 모르겠다.

우선 설명을 해보자면 python에는 흔하게 사용되는 정수 값들은 항상 그 object가 생성되어 있다고 한다.

여기서 흔하게 사용되는 정수 값이 바로 -5~256범위의 수이다.

이 범위의 값들은 항상 object가 생성되어있기 때문에 id()를 활용하여 메모리주소를 찍어보아도 이미 생성되어있는 메모리주소만을 보여줄 뿐이다.

우리가 이 값을 사용하는 경우에는 이미 만들어진 값들을 참조할 뿐이라고한다.

반면에 이 범위를 벗어나는 값들은 호출이 이루어질 때마다 object를 생성하기 때문에 그 메모리 값이 다르게 변화한다고 한다.

![result1](./cap1.PNG)
![result2](./cap2.PNG)