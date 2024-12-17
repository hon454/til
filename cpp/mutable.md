# mutable

`mutable`은 const 함수 내에서 멤버 변수를 수정할 수 있게 해주는 키워드다. `const` 함수는 객체의 상태를 변경하지 않도록 보장하지만, `mutable`로 선언된 변수는 예외적으로 수정할 수 있다.

이를 통해 함수 호출 횟수나 캐시된 값 등 내부 상태를 추적하거나 성능 최적화를 할 수 있다.

단, `mutable`은 `const` 함수 내에서만 수정할 수 있으며, `const`가 아닌 함수에서는 일반 변수처럼 동작한다.


```cpp
class Counter
{
public:
    int GetCount() const
    {
        m_calls++;  // mutable 변수는 const 함수 내에서도 수정 가능
        return m_count;
    }

    void Increment() { m_count++; }

private:
    int m_count = 0;
    mutable int m_calls = 0;  // const 함수 내에서도 수정 가능
};
```
