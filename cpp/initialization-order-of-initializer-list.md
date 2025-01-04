# 초기화 리스트의 초기화 순서

초기화 리스트의 초기화 순서는 초기화 리스트의 작성 순서가 아닌 **멤버 변수 선언 순서**에 따른다.

멤버 변수를 선언 순서에 맞게 초기화해야 예기치 않은 동작을 방지할 수 있다.

```cpp
#include <iostream>

class Example {
private:
    int a;
    int b;

public:
    Example(int x, int y) : b(y), a(x) {
        std::cout << "a: " << a << ", b: " << b << std::endl;
    }
};

int main() {
    Example ex(10, 20);  // a: 10, b: 20
    return 0;
}
```
