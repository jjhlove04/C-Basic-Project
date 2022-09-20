# C# Baics Project

---

## **목차**

`목차의 내용을 선택 시 해당 항목으로 이동합니다.`

<!--챕터 1-->
<details>

<summary><a href="#Chapter" > Chapter 1 </a></summary>

<strong>[Chapter 1 - 1] [C#의 기본](#c의-기본과-객체지향에-대해-알아봅시다)</strong> </br>
<strong>[Chapter 1 - 2] [자료형](#자료형을-먼저-살펴-봅시다)</strong>

</details>

<!--챕터 2-->
<details>

<summary><a href="#Chapter" > Chapter 2 </a></summary>

<strong>[Chapter 2 - 1] [변수](#변수에-대해-알아봅시다) </strong></br>
<strong>[Chapter 2 - 2] [형 변환](#형-변환에-대해-알아봅시다) </strong></br>
<strong>[Chapter 2 - 3] [연산자](#산술-연산자에-대해-알아봅시다) </strong></br>
<strong>[Chapter 2 - 4] [조건문](#형-변환에-대해-알아봅시다) </strong></br>

</details>

<!--챕터 3-->
<details>

<summary><a href="#Chapter" > Chapter 3 </a></summary>

<strong>[Chapter 1 - 1] C#의 기본</strong></br>
<strong>[Chapter 1 - 2] 자료형</strong>

</details>

<!--챕터 4-->
<details>

<summary><a href="#Chapter" > Chapter 4 </a></summary>

<strong>[Chapter 1 - 1] C#의 기본</strong></br>
<strong>[Chapter 1 - 2] 자료형</strong>

</details>

---

# Chapter 1 - 1

##### `C#의 기본과 객체지향에 대해 알아봅시다.`

### What is C# ?

<strong>C</strong> 와 <strong>C++</strong>의 강점, 비주얼 베이직의 편의성을 결합하여 만든 <strong>객체지향 프로그래밍</strong> 언어입니다. <strong>닷넷</strong>을 기반으로 하여 <strong>웹 프로그래밍, 데이터 베이스 프로그래밍, 서버 - 클라이언트 개발, 사물인터넷 (IoT)</strong> 와 같은 거의 모든 프로그래밍에서 사용되는 강력한 언어입니다.

### 객체지향이란?

C#에 꼬리표 처럼 따라오는 <strong>객체지향성</strong> 입니다. 객체지향이란 <strong>필요한 데이터를 추상화시켜 상태와 행동을 가진 객체( Object )</strong> 로 만들고 <strong>객체끼리의 상호작용을 통해 로직을 구성</strong>하는 프로그래밍 기법입니다.

#### **객체지향에는 5대 원칙이 존재합니다.**

1. 클래스 + 인스턴스 ( 객체 )
2. 캡슐화
3. 상속
4. 추상화
5. 다향성

## 1) **클래스 와 인스턴스**

<strong>클래스</strong> - 속성과 행위를 변수와 매서드로 정의한 것
<strong>인스턴스</strong> - 클래스에서 정의한 것을 토대로 실제 메모리에 할당된 객체

## 2) **캡슐화**

- 데이터를 은닉하고 접근하는 기능을 노출시키지 않는다.
- 데이터의 구조와 데이터를 다루는 방볍을 결합시켜 묶는다.

쉽게 캡슐 알약 안에 내부약물을 보호하는 기능을 예로 들면 이해하기 쉽습니다.

캡슐화의 접근을 제어하는 접근지정자 목록입니다.

- public : 모두가 접근 가능한 지시자
- protected : 상속되거나 같은 패키지 내에서만 접근 가능
- private : 본인만 접근 가능

## 3) **상속**

- 상속은 상위 클래스의 내용을 하위 클래스가 물려 내려받는 것 입니다. 쉽게 말하면 부모 클래스의 내용을 자식 클래스에 물려주는 것 과 같습니다.

상속은 먼저 이미지를 보고 가도록 합시다.

<center>
<img src="./images/InheritanceImage.png" />
</center>

이처럼 공통으로 가지고 있는 요소를 부모 클래스로 묶고 개개인의 특성을 자식클래스의 구현하도록 합니다. 가장 기본적인 C#의 프로그래밍 구조라고 할 수 있습니다.

<center>
<img src="./images/example2.png" />
</center>
위의 이미지 처럼 <strong>적</strong> 클래스가 공통으로 가지고 있는 부모 클래스이고, 특성을 가지고 있는 자식 클래스인 미니언들의 클래스에 상속 받아 사용중인 예제입니다.

## 4) **추상화**

- 추상화란 객체의 <strong>공통 속성</strong>을 뽑아내는 것 입니다.

예를 들어 피격을 당했을 때, 적과 플레이어는 데미지를 받는 것 이 것은 공통으로 할당된 이벤트 입니다. 우리는 초점을 <strong>피격을 누가 당했는지</strong> 가 아닌 <strong>"데미지를 받는 것"</strong> 에 대해 추상화를 했다는 것 입니다.

한마디로 사용하기 쉽게 <strong>"추상화"</strong> 한 것 입니다.

---

# Chapter 1 - 2

##### `자료형을 먼저 살펴 봅시다.`

## 1) <strong>정수형</strong>

- sbyte - 부호 있는 8비트 정수
- byte - 부호 없는 8비트 정수
- short - 부호 있는 16비트 정수
- unshort - 부호 없는 16비트 정수
- int - 부호 있는 16비트 정수
- unint - 부호 있는 32비트 정수
- long - 부호 있는 64비트 정수
- unlong - 부호 없는 64비트 정수

이처럼 정수형에만 여러가지 자료형이 있습니다. 왜냐하면 상황에 맞는 자료형을 사용해야 합니다. <strong>자료형에 따라 할당되는 메모리의 크기가 다르기</strong> 때문에 각 상황에 맞는 자료형을 선택해서 사용해야 합니다. 예를 들어 100명의 학생수를 담을 수 있는 변수를 선언해 보겠습니다.

```cs
// 적절한 자료형 활용
sbyte studentCount = 100;
byte studentCount = 100;

// 부적절한 자료형 활용
int studentCount = 100;
```

아래와 같이 적절한 자료형 활용은 불필요한 메모리를 줄이는 가장 기초적인 방법 중 하나 입니다.

## 2) <strong>실수형</strong>

- float - 32비트
- double - 64비트
- decimal - 128비트

소수점을 포함하기 시작하면 <strong>정확한 수의 표현이 아닌 근사치를 표현</strong>하는데 더 특화 되어 있습니다. 소수점 이하의 모든 수를 표현하는 것은 비효율적 이기 때문에 아주 작지만 조금의 오차범위가 생길 수 밖에 없다. decimal 같은 경우 천문학과 같은 분야에서 <strong>한치의 오차가 허용되지 않을 때</strong> 사용하는 자료형입니다.

## 3) <strong>문자(열)형</strong>

- char - 유니코드 16bit ( 개당 2byte )
- string - 유니코드 16bit 조합

<strong>"유니코드"</strong>란? : 유니코드는 모든 나라의 언어를 표현하기 위해 나온 코드체계, 운영체제, 나라, 프로그램, 언어에 상관없이 문자마다 고유한 코드 값을 제공하는 방식.

## 4) <strong>부울린형</strong>

- bool - 8bit ( 1 byte )

오로지 참과 거짓을 판별할 때 사용하는 자료형 입니다.

---

# Chapter 2 - 1

##### `변수에 대해 알아봅시다.`

변수는 자료를 담는 그릇이자 이름표 입니다.

```cs
int a; //와 같이 int 자료형을 가진 변수 a를 생성
a = 10; //a를 선언 후 값을 할당

int b = 10; //와 같이 int 자료형을 가지고 10이라는 값을 가지고 있는 변수 b를 생성
```

변수를 선언하고 값을 할당하는 방법을 알아보았습니다.
변수에 값을 배정하는 <strong>시점을 조절하여</strong> 프로그래밍 할수 있습니다. 값을 선언과 동시에 배정하여 사용할수 있고 선언 후 다음줄에서 배정 할 수도 있습니다.

#### `문자열 과 문자 선언시`

```cs
char mark = '!';

string name = "지뇽이";
```

문자로 할당된 곳은 ('') 작은 따옴표를 사용해서 값을 배정하지만 문자열은 ("") 큰따옴표를 사용해서 값을 배정하게 됩니다.

## <strong>변수값 출력 방법</strong>

우리는 선언한 변수를 확인하기 위해 출력해 볼 필요가 있습니다.
C#에는 Console을 활용하여 출력이 가능합니다. C# 에는 두가지 출력문을 제시합니다. `write` 와 `writeLine` 입니다. 둘의 차이는 <strong>커서의 위치가 줄바꿈을 하냐, 하지 않느냐</strong> 입니다.

```cs
Console.Write("지뇽이"); //커서의 위치

Console.WriteLine("지뇽이");
//커서의 위치
```

---

#### 그 다음 알아 볼 출력 방법은 <strong>PlaceHolder</strong> 와 <strong>Interpolation</strong> 입니다. Placeholder 에 대해 먼저 설명하겠습니다.

#### <strong>`Placeholder`</strong>

placeholder 를 적용한 출력 방법은 다음과 같습니다.

```cs
string name = "지뇽";
Console.WriteLine("제 이름은 {0} 입니다.", name);
```

이렇게 `{숫자}`를 넣어서 출력으로 사용할 수 있습니다 `숫자`는 뒤따르는 , 다음의 변수중 몇 번째 변수 값을 가져올지 정합니다.
첫번째가 1이 아닌 0으로 시작합니다.

### `Placeholder 예제`

```cs
int x = 120;
float y = 3.14;
char z = 'A';

///x,x,x 값 출력
Console.WriteLine("{0} {0} {0}",x,y,z);
// x,y,z 값 출력
Console.WriteLine("{0} {1} {2}",x,y,z);
//z,x,y 값 출력
Console.WriteLine("{2} {0} {1}",x,y,z);
```

#### <strong>`Interpolation`</strong>

interpolation 을 적용한 출력 방법은 다음과 같습니다.

```cs
string name = "지뇽";
int age = 19;
Console.WriteLine($"이름 = {name} 나이 = {age}");
```

이렇게 앞에 `$`를 쓰면 `{}`안에 변수명을 써주면 바로 변수의 값을 불러 올 수 있는 출력 방법 입니다.

#### `Interpolation 예제`

```cs
int a = 1234;
float A = 12.34;

//소문자 a의 값을 출력
Console.WriteLine($"a = {a}");

//대문자 A의 값을 출력
Console.WriteLine($"A = {A}");
```

## <strong>변수명 짓는 방법</strong>

변수의 이름은 정말 중요합니다. 변수이름을 보고 어디에 어떻게 쓰이는 변수인지 한번에 알아차릴 수 있는 변수이름을 짓는것이 핵심입니다.
이름을 지을 때 자신의 역활을 설명하도록 만들어야 하며 이는 변수 뿐만 아니라 상수, 함수, 클래스 등 여러가지에 적용됩니다.

가장 일반적으로 사용하는 변수 이름을 짓는 3가지 규칙을 소개하겠습니다.

##### 1. 변수명에는 줄임말보다 한번 보고 바로 이해할 수 있는 이름을 사용할 것.

##### 2. 변수명에는 밑줄(\_)이나 하이픈(-)을 사용하지 말 것

##### 3. 변수병에는 단수형 명사를 사용하고, 여러 단어의 조합인경우 camelCase를 사용할 것

---

#### `camelCase` 와 `PascalCase`

`camelCase`는 주로 여러단어의 조합으로 된 변수의 이름에 사용된다.
예시) userName, rankSystem, partyUser

`PascalCase`는 주로 클래스나 인터페이스의 이름으로 사용되는데 첫번째와 띄어쓰기가 되는 부분이 둘다 대문자인 특성을 지니고 있다.
예시) UserData, PlayerData, OnDamage

---

# Chapter 2 - 2

##### `형 변환에 대해 알아봅시다.`

프로그래밍을 하다가 보면 문자형을 int형이나 float형으로 바꾸어서 쓸 경우가 존재합니다.
반대로 숫자를 문자형으로 변환하여 사용하는 경우도 존재합니다.

필자가 쓰는 유니티에서도 Text라는 곳에 string 으로 넣어주어야 하기 때문에 int 나 float 으로 된 자료형을 변환해서 사용합니다.

### ToString() 과 Parse()

Convert.ToXXX 와 같은 변환 함수도 있지만 여기에선 캐스팅과 ToString 과 Parse만 다루도록 하겠습니다.

```cs
Console.WirteLine("숫자를 입력하세요 :")
int a = int.Parse(Console.ReadLine()); //int형으로 문자형을 변환해서 입력받기

//EX)
double.Parse()
float.Parse() //앞에 자료형.Parse() 사용가능
```

### <U> Casting (캐스팅)</U>

사실상 가장 간단한 형 변환 방법 입니다. 내가 바꾸고자 하는 변수 앞에 (원하는 자료형)을 붙여준다면 형 변환이 가능합니다.

```cs
int i = 10;
double d = 0.1;

float a = 0.000001f;

i = (int)a;
d = (double)a;
// output>>>
//0
//9.999999747378752E-05
```

**<U>주의! 캐스팅은 숫자형을 문자형으로 바꿀수 없습니다.</U>**

## **<U>Const (상수)</U>**

##### `상수에 대해 알아봅시다.`

절대 변하지 않는 수가 있습니다. 흔히 알고있는 PI(파이)는 하늘과 땅이 무너져도 3.141592... 입니다.
이처럼 우리가 프로그래밍을 하게 되면 절대 변하지 않아야 할 값이 존재하는 상황이 존재합니다.

const를 사용하여 절대 변하지 않는 상수를 만들어봅시다.

```cs
//잘못된 예
const int a;
a = 10;
//올바른 예
const int a = 10;
```

---

# Chapter 2 - 3

## **<U>Arithmetic Operator (산술 연산자)</U>**

##### `산술 연산자에 대해 알아봅시다`

중요한 사칙연산을 수행하는 기호들 입니다. 기본 기능이라고 할 수 있을만큼 중요합니다.
프로그래밍에서 사칙연산은 우리가 알고있는 수학의 계산과 전혀 다르지 않습니다.

- 더하기 (+) : 수를 더하는 기능을 합니다.
- 빼기 (-) : 수를 빼는 기능을 합니다.
- 곱하기 (\*) : 수를 곱하는 기능을 합니다.
- 나누기 (/) : 나누고 몫을 가져옵니다.
- 나누기 (%) : 나누고 나머지를 가져옵니다.

#### **<U>모든 계산은 산술연산의 우선순위를 따릅니다 :)</U>**

```cs
int a = 3, b = 5, c = 4;

//앞에서 부터 순차적으로 계산
Console.WriteLine(a+b-c);
>> 4

//곱셈부터 계산
Console.WriteLine(a+b*c);
>> 23

//괄호 먼저 계산
Console.WriteLine(a*(c-b));
>> -3
```

##### 컴파운드 연산자

컴파운드는 (=)입니다. = (컴파운드) 와 산술연산자를 섞어 더 간단한 식을 만드는 것을 말합니다.

```cs
int a = 10;

//a = a + 10과 같습니다
a += 10;
>> 20

//a = a * 2와 같습니다
a *= 2;
>> 40

//a = a / 10과 같습니다
a /= 10
>> 4
```

##### 증감 연산자

제어문 for문에서 가장 많이 볼수있는 연산자입니다. (++) 와 (--)를 사용해 1을 더하고 빼는 연사자입니다. 변수의 앞에 사용하느냐 뒤에 사용하느냐에 따라 결과가 크게 달라지니 유의하여 사용해야합니다.

```cs
int a = 1;

//먼저 +1 을 하고 넘겨주기 때문에 2가 출력
a = ++a;
Console.WriteLine(a);
>> 2

//a를 먼저 전달받고 그다음에 +1을 하기 때문에 1이 출력
a = a++;
Console.WriteLine(a);
>> 1
```

---

# Chapter 2 - 4

##### `프로그래밍 코드의 흐름제어에 대해 알아봅시다`

## 조건문

조건문은 문장의 구조를 이어주는 다리와 같은 역할을 합니다. 가위바위보를 할 때, 내가 가위를 낸 경우에 이겼을 때와 졌을 때 결과를 다르게 출력해야하는 상황에서 승패를 판가름해주는 역할을 합니다. 조건문은 참과 거짓으로 문장을 구분할때 사용하게 됩니다.

- if 문
- switch 문
- try - catch 문

## if 문

if 문은 조건이 참일 경우에만 {코드 블럭} 안에 있는 명령을 수행한다. 반드시 중괄호 {} 로 감싸 주어야 하는데 안에 묶여있는 명령의 집합을 코드 블럭이라고 합니다.
if문은 else 와 같이 사용하는데 if문만 사용해도 된다. 즉 선택사항입니다.

```cs
int a = 10;
int b = 5;

if(a > b)
{
  Console.WriteLine("a 가 b 보다 큽니다.");
}
else //a 가 b보다 크지 않다면
{
  Console.WriteLine("a 가 b 보다 크지 않습니다.");
}

>>> a 가 b 보다 큽니다.
```

위처럼 a 가 더 큰게 참일때 출력을 하는 조건문을 작성했습니다. 그래서 출력 결과도 a가 b보다 크다고 나왔습니다.
else는 무엇이냐, if로 거르지 못한 나머지 조건들을 포함하고 있다고 생각하면 됩니다. a 가 b보다 큰 경우가 아닌 모든 경우를 생각하면 됩니다.

+else if 문을 추가로 서술 하겠습니다. <strong>if 문에서 조건이 거짓인 경우 바로 else 로 넘어가기 보다,</strong> 다른 부합한 조건이 없는지 한번 더 확인 할 수 있습니다.

```cs
int a = 10;
int b = 5;

if(a > b)
{
  Console.WriteLine("a 가 b 보다 큽니다.");
}
else if(a == b)
{
  Console.WriteLine("a 와 b 가 같습니다.");
}
else //a 가 b보다 크지 않다면
{
  Console.WriteLine("a 가 b 보다 크지 않습니다.");
}

>>> a 가 b 보다 큽니다.
```

**<U>주의할점.</U>** if - else if - else 순서로 명령문 구조를 작성해야 합니다. 순서가 절대 바뀌면 안됩니다.

## Switch 문

if문에 비해 가독성이 좋은 switch문을 자주 사용합니다.
기본 구조는 switch(a) a의 조건에 따라 결과를 출력합니다. case : 와 case 안에 break; 로 기본 구성이 됩니다.

```cs
int x = int.Parse(Console.ReadLine());
switch(x)
{
  case 1:
    Console.WriteLine("x = 1 입니다.");
  break;
  case 2:
    Console.WriteLine("x = 2 입니다.");
  break;
  case 3:
  case 4:
    Console.WriteLine("x는 3 아니면 4입니다.");
  break;
  //default:
  break;
}
```

## While 과 do-while 문

먼저 이제 우리가 또 많이 사용할 반복문이 등장헀습니다. 말 그대로 일정 조건동안 반복하는 명령을 수행하게 해주는 문법입니다.

```cs
int x = 1;

while(x < 10)
{
  Console.WriteLine(x);
  x++
}
>> 1,2,3,4,5,6,7,8,9
```

()안에 조건을 만족하는동안 while문이 실행된 것을 확인 할수 있습니다. 다음 반복문은 while에 do 가 추가된 do-while문 입니다. 쉽게 말하면 <strong>반복을 하기위해 먼저 검사하는 구조</strong>라고 생각 하시면 쉽습니다. 예제를 살펴보도록 하겠습니다.
