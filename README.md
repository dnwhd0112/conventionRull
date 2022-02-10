# conventionRules
컨벤션 규칙 가이드

* Fundamentals [기본]
  * 무엇에, 어떨 때 사용하는 지에 대한 명확함이 중요. Method나 property(클래스, 구조체, 열거형에 소속된 변수 및 속성)의 쓰임을 명확하고 concise(불필요한 정보없이 깔끔하게, 구체적이고 간결하게)하게 하라.
  * 쾌함(Clarity)이 짧음(brevity)보다 중요하다.
  * 선언마다 documentation comment 작성하라.

* Naming
  * 모호성(ambiguity)를 피하기 위해 필요한 모든 단어를 포함하게 하라. (읽는 사람이 이게 뭔지, 뭘하는 것인지 헷갈리지 않게 이름지어라)
  * 필요없는 단어는 없애라. (예를 들어 Element 매개변수로 받아 remove하는 함수를 removeElement라고 짓지 않고 remove라고만 해도 된다 )
  * 변수, 매개변수, associated type의 이름은 그들의 타입보다는 역할에 따라 이름을 지어라(인사를 하는 변수라면 string이라고 이름짓지 말고 greeting 이라고 이름 짓는다)
  * Type information이 적은 것을 보완해서 parameter의 역할을 분명히 한다. Weakly typed parameter에 역할을 묘사하는 명사를 붙인다


----

1. 함수 혹은 조건문을 작성
```
func funcName() -> [Int] {
    var userArray : [Int] = [0, 0, 0]
    var userName: String
    
    for index in 0...userArray.count {
        if !userArray.contains(0) {
            print("message")
        }
    }
    return randomNumbers
}
```
* 띄어쓰기, 들여쓰기 유의
* 변수는 바로 함수 밑에 오도록
* 변수 선언하고 한 줄 넘기기


