# 경기게임마이스터고등학교 학생들을 위해서 만든 C#의 입문 가이드라인

> ~~**아직 미완성**~~

## 목차

<details>

<summary><a href="#프로그래밍을-시작하기-전에"> 1. 프로그래밍을 시작하기 전에 </a></summary>
<br>

- [1-1 이걸 왜 해야 하는 걸까](#이걸-왜-해야-하는-걸까)
- [1-2 앞으로 배우게 될 것의 간단 설명](#앞으로-배우게-될-것의-간단-설명)
- [1-3 공부하게 될 곳의 환경 설정과 기본 파일구조](#공부하게-될-곳의-환경-설정과-기본-파일구조)
  
</details>
<details>

<summary><a href="#처음-보게-되는-프로그램"> 2. 처음 보게 되는 프로그램 </a></summary>
<br>

- [2-1 Hello World!](#안녕-세상)
- [2-2 프로그램 뜯기](#프로그램-뜯기)
  
</details>
<details>

<summary><a href="#데이터-보관"> 3. 데이터 보관 </a></summary>
<br>

- [3-1 변수](#변수)
<details>
  <summary><a href="#값-형식과-참조-형식"> 3-2 값 형식과 참조 형식 </a></summary>
  <br>
  
  - - [3-2-1 스택과 값 형식](#스택과-값-형식)
  - - [3-2-2 힙과 참조 형식](#힙과-참조-형식)
</details>
  
- [3-2 기본 자료형](#기본-자료형)
  
- [3-3 조건문](#조건문)
  
- [3-4 반복문](#반복문)
  
</details>

# 프로그래밍을 시작하기 전에

> 이것을 읽는 독자가 노트북과 마우스를 가지고 있다는 가정하에 진행합니다.  
> 만약 C#을 시작하기 위한 'Visual Studio 2019'가 없다고 해도  
> [1-3](#공부하게-될-곳의-환경-설정과-기본-파일구조)에서 설치 방법을 알려 줄 예정이니  
> 걱정하지 말고 진행하셔도 됩니다.  
> 만약 정확하고 자세한 정보를 얻고 싶으신다면   
> https://docs.microsoft.com/ko-kr/dotnet/csharp/tour-of-csharp  
> 이곳에서 확인해주세요

- - -
## 이걸 왜 해야 하는 걸까

이 학교는 **게임개발자**를 양성하는 학교이며  
학생들이 개발자를 목표로 하고 있다고 생각하며 학교의 커리큘럼이 가춰져 있습니다.  

그리고 무엇보다 학교 프로젝트는 C#을 주로 사용합니다.

하지만 나는 아트나 기획을 목표로 하고 여기에 왔는데? 라고 할 수 있는데  
당연하게도 프로그래밍을 할 수 있는 기획자 또는 아트라면 자신의 몸값이 상승하겠죠?  
그러므로 나중에 후회하지 않도록 지금 하도록 합시다  

- - -
## 앞으로 배우게 될 것의 간단 설명

우리는 앞으로 'C#'을 주력언어로 해서 배울 것입니다.  

![새 프로젝트](https://user-images.githubusercontent.com/70933806/173963206-3ffe1565-dd75-45fa-959a-468e3f0dd829.png)

C#은 프로그래밍 언어입니다.  
프로그램을 작성하기 위해서 사용하는 언어이지요

![새 프로젝트 (1)](https://user-images.githubusercontent.com/70933806/173963611-c801d7a0-d2b9-4da3-8455-3372c6cd4256.png)

조금만 프로그래밍 언어에 대해서 찾아보면 알다시피  
프로그래밍 언어의 종류는 매우 많습니다.

근데 왜 하필 많고 많은 프로그래밍 언어들 중 C#을 배워야 하는 의문이 들 수 있는데,  
그 이유는 크게 2가지가 있습니다.  
첫 번째는 Unity 엔진과 같이 사용되고  
두 번째는 난이도가 상대적으로 쉬워서입니다.  
 
이 학교에 처음 들어오게 되었을 때 대부분의 학생들이 프로그래밍을 처음 접한 상태 일 것 입니다.  
일단 저희는 그랬으니까요  
그래서 처음 배우는 입문 개발자들을 위해서  
상대적으로 난이도가 낮고 배우기 쉬운 언어인 C#을 고른 것 입니다.

물론 상대적으로 쉬운 것일 뿐, 매우 힘든 과정을 겪어가며 배울 것 입니다.  

이 학교에 온 학생들 대부분이 게임 개발자를 목표로 해서 왔을 것일 텐데  
이 목표를 이루기 위해서는 넘겨야 하는 벽입니다.

자신이 능력 있는 사람이 되고 싶다면, 열심히 해야겠죠?  

- - -
## 공부하게 될 곳의 환경 설정과 기본 파일구조

앞에서 공부하게 될 언어와 학교의 목표를 알아보았는데,  
이제는 본격적인 환경 설정을 할 차례입니다.  

1. 웹 브라우저로 https://visualstudio.microsoft.com/ 에 접속한 후, "Visual Studio" 항목에서 [Visual Studio 다운로드]를 선택하고 [Community 2019]를 클릭하세요.

![화면 캡처 2022-06-16 094136](https://user-images.githubusercontent.com/70933806/173965317-4f451c49-ed51-4f57-bf4e-e3c0a60d598e.png)

2. 다운로드 받은 파일을 실행하세요. 설치 프포그램이 다음과 같이 메시지를 띄우면 계속 버튼을 클릭합니다.

![화면 캡처 2022-06-16 094143](https://user-images.githubusercontent.com/70933806/173965343-9afffd73-9236-487c-b97f-f9cce35676d0.png)

3. 설치 프로그램이 옵션을 물어볼 겁니다. 우리가 필요한 것은 ".NET 데스크톱 개발"이며 "Unity를 사용한 게임 개발"도 원하시면 같이 선택하고 설치 버튼을 클릭하세요.

![화면 캡처 2022-06-16 094149](https://user-images.githubusercontent.com/70933806/173965369-4f4261bf-df2c-407c-8002-4d2b656c49f3.png)

4. 설치가 완료되었다면 시작 메뉴에서 Visual Studio를 찾아 실행하세요.

5. 비쥬얼 스튜디오를 처음으로 실행하면 테마를 선택하는 화면이 나타날 것 입니다. 취향에 맞는 테마를 고르고 시작 버튼을 클릭하면 비주얼 스튜디오가 시작됩니다.

- - -
# 처음 보게 되는 프로그램

> 여기서 부터는 자신이 직접 해가며 배워나가야 합니다

- - -
## 안녕 세상 
> Hello, World!

이제 코드를 작성하기 위한 간단한 프로그램을 만들어보겠습니다.

1. 비주얼 스튜디오 실행하기

2. 실행이 되었다면 "새 프로젝트 만들기" 버튼을 클릭하기

![1](https://user-images.githubusercontent.com/70933806/173972074-0a0ba53b-45bf-41ef-8156-677979b04c36.png)

3. 잘 띄어졌다면 C#으로 선택 한 뒤 "콘솔 애플리케이션"를 선택합니다.

![2](https://user-images.githubusercontent.com/70933806/173972171-7317f074-3552-4678-bec3-313f7ac025ae.png)

4. 나타난 창에서 프로젝트의 이름을 마음대로 설정하고 만들기를 클릭합니다.

![3](https://user-images.githubusercontent.com/70933806/173972218-7c669666-ef01-494f-bd13-c007d0d595d6.png)

5. 여기까지 진행했다면 다음과 같이 코드 편집기와 솔루션 탐색기가 나타날 겁니다.

![4](https://user-images.githubusercontent.com/70933806/173972284-6411a315-8043-4c33-9557-1cc48a70863f.png)

이제부터는 소스 코드를 작성해야 합니다. 코드 편집기에 밑의 코드를 작성해보세요!  

```cs
using System;
using static System.Console;

namespace Hello
{
  class MainApp
  {
    static void Main(string[] args)
    {
      WriteLine("Hello World!");
    }
}
```

> 컴파일 설명 따로 넣기  
소스코드를 모두 입력했다면 이제는 컴파일을 해야 합니다.   
비주얼 스튜디오의 "빌드" -> "솔루션 빌드" 메뉴를 클릭해서 컴파일을 수행합니다.  
소스코드에 문제가 없다면 실행파일을 생성하겠지만, 문제가 있다면 에러를 띄울 것입니다.  
오류가 나왔다면 다시 한번 코드를 비교하며 어디서 잘못되었는지 찾아보길 권장합니다.


이제 실행파일을 확인하러 갑시다.  
밑처럼 "파일 탐색기에서 폴더 열기"를 클릭하면 프로젝트의 경로로 바로 이동 할 수 있습니다.

![5](https://user-images.githubusercontent.com/70933806/173972349-b8ec7e45-d815-4779-ab63-964ceed8d4a7.png)

정상적으로 빌드가 되었다면 밑의 경로안에 Hello.exe가 만들어 졌을 것 입니다.

![6](https://user-images.githubusercontent.com/70933806/173972402-1c6912ee-ac02-41ad-b18e-6d0b82179b1b.png)

이제는 프로그램을 실행 시킬 차례가 왔습니다.  
1. "Windows + R" 단축키를 누르고 "cmd"를 입력한 뒤 엔터를 누릅니다.  
2. 이 창에서 "cd [Hello.exe가 있는 파일 경로]" 를 입력합니다.  
3. 마지막으로 "Hello.exe"를 입력합니다.

![7](https://user-images.githubusercontent.com/70933806/173972440-269bede9-8c92-48e6-8dcd-36833f57f0b8.png)

여기까지 하셨다면 성공적으로 진행하신겁니다.  
이제는 지금 작성한 프로그램이 어떤 것인지 확인하러 갈 것입니다. 

- - -
## 프로그램-뜯기

이제 아까 작성한 소스코드를 하나하나 설명할 차례입니다.  
그런데 전에 작성한 코드랑 뭔가 다른 부분이 있습니다.  
다 이해를 돕기 위해서 있는 코드므로 무시하고 넘어가 주세요!  

```cs
  using System;
  using static System.Console;

  namespace Hello
  {
      class Program
      {
          // 프로그램의 
          static void Main(string[] args)
          {
              System.Console.WriteLine("Hello World!");

              Console.WriteLine("Hello World!");

              WriteLine("Hello World!");
          }
      }
  }
```

> using System;

using System; 은 보이는 것과 다르게 총 3개의 요소로 나눌 수 있습니다.  
'using', 'System', ';'(세미콜론) 이 각각 개별적인 기능을 가지고 있기 때문이죠.  

첫 단어 using은 C#의 키워드(C# 언어에서 미리 정의되어 있는 특별한 단어) 중 하나 입니다.  
using 하면 뭔가를 사용한다는 의미가 떠오를텐데 여기서도 마찬가지로 뒤에 있는 System을 사용하겠다고 한 것입니다.  

그럼 System은 무엇인가하면 클래스(나중에 설명)를 모아놓은 네임스페이스(이건 잠시 후에 설명합니다) 입니다.  

따라서 "using System"은 System 네임스페이스 안에 있는 클래스들을 사용한다는 것을 알려줍니다.  
마지막으로 ';'은 문장의 끝을 알리는 기호라서 작성한 것입니다.

> using static System.Console;

이 문장은 'using', 'static', 'System.Console', ';' 으로 총 4가지로 나뉘어 있습니다.  
'System.Console' 먼저 설명하고 앞으로 다시 돌아오겠습니다. 

System은 아까 앞에서 말했듯이 네임스페이스 입니다.  
근데 '.Console'이 붙으면 System 네임스페이스 안에 있는 Console 클래스를 의미하게 됩니다.

그럼 'using static'은 무엇이나면 'Console' 클래스 안에 있는 "static 멤버"(정적 멤버 이것도 뒤어서 설명)를 사용하겠다고 명시하는 것입니다.  

> namespace Hello { }

네임스페이스는 앞에서 말한 클래스와 같은 기능들을 하나의 이름으로 묶는 일을 합니다.  

네임스페이스를 만들 때는 다음과 같이 namespace 키워드를 사용하며 그 뒤에 이름이 붙습니다.  
그리고 '{'와 '}' 는 이 네임스페이스에 소속할 클래스등이 들어가게 됩니다.

```cs
namespace 쓰고_싶은_이름
{
  // 각종 기능들
}
```

다시 우리가 작성한 코드를 보면 Hello라는 네임스페이스 안에 Program이라는 클래스를 담고 있다는 것을 알 수 있습니다.  
다른 곳에서 Program 클래스를 사용하기 위해선 'using Hello'를 통해 네임스페이스를 가져오거나, 'using static Hello.Program'을 통해 클래스의 정적 멤버를 사용할 수 있습니다.

> class Program { }

대강 감이 잡혔겠지만 class 라는 키워드로 Program이라는 이름을 가진 클래스를 만듭니다.  
그래서 계속 언급되는 클래스가 무엇이냐면 C# 프로그램을 구성하는 기본 단위로써 데이터와 데이터를 처리하는 기능(이걸 메소드라고 불러요)으로 이루어집니다.  
C# 프로그램은 최소한 한개의 클래스로 이루어지며 수많은 클래스로 구성되기도 합니다.

우리가 작성한 코드를 보면 Program이라는 클래스 안에 Main 메소드가 있습니다.

클래스에 대해서는 나중에 더욱 자세하게 설명하도록 하겠습니다.

> // 프로그램의 시작

'//'으로 시작하는 코드를 주석이라고 합니다.  
주석은 소스코드에 아무런 영향으로 주지 않고 오직 사람이 볼 수 있는 메모로써 기능을 합니다.  

한줄 이상의 주석을 작성하고 싶다면 '//'을 줄마다 작성하거나, '/* 주석 내용 */'으로도 적성 할 수 있습니다.

> static void Main(string[] args) { }

'static void Main(string[] args)'는 앞에서 말했듯이 메소드 입니다.  
이 메소드는 특별하게도 프로그램의 진입점으로 시작되면 실행하고, 이 메소드가 종료되면 프로그램도 종료합니다.  
그래서 모든 프로그램은 반드시 Main이라는 메소드를 가지고 있어야 합니다.

가끔 메소드라는 단어 대신 함수, 서브루틴으로 불리우는 경우도 있으니 혼동하지 않도록 합시다.  

이제 'static', 'void', 'Main(string args[])' 로 나눠서 설명하겠습니다.

static은 한정자 (프로그래밍 언어에서 사용되는 다른 요소를 꾸며주는 역할) 로써 메소드 또는 변수를 꾸며줍니다.  
프로그램의 각 요소는 코드가 실행되는 시점에서 메모리에 할당되는 반면, static 키워드로 수식된 코드는 프로그램이 처음 구동 될때부터 진작에 메모리에 할당 된다는 특징이 있습니다.

void는 메소드의 반환형식 입니다. 반환형식에 대해서는 나중에 자세히 설명하겠지만 간단히 설명하면 void의 뜻은 '비어 있는'이라는 뜻으로 이 메소드가 아무것도 반환하지 않는 다는 것을 알려주는 역할을 합니다.

Main은 메소드의 이름이고 메소드의 이름 뒤에 있는 괄호와 그 사이어 있는 코드는 메소드에 입력되는 매개변수입니다.  
메소드가 실행되게 되면 '{'부터 시작해서 '}'을 만날 때까지 차근차근 실행해 나갑니다.

> System.Console.WriteLine("Hello World!");  
> Console.WriteLine("Hello World!");  
> WriteLine("Hello World!");  

한번에 3개의 코드를 설명하면 3개의 코드들 모두 "Hello World!"라는 문자열을 출력하는 메소드를 실행한 것 입니다.  
WriteLine이 함수 이름이며 괄호 안에 있는 "Hello World!"가 매개변수의 값이죠  

여기서 3개의 차이점은 System과 Console인데  
System은 네임스페이스이고 Console은 클래스라는 것을 설명 했습니다 
앞에서 설명한 'using System;'을 작성하면 'Console.WriteLine("Hello World");' 까지 가능하며  
using static System.Console;'을 작성하면 'WriteLine("Hello World!");' 까지 생략이 가능합니다.  
아무 생략 코드를 작성하지 않는다면 'System.Console.WriteLine("Hello World!");'으로 출력 메소드를 호출해야 하죠



이상으로 우리가 작성한 코드를 뜯고 맛보았습니다.  
다음으로는 프로그램의 기본인 데이터에 관해서 다루도록 하겠습니다.
- - -
# 데이터 보관

> 앞에서 우리가 앞으로 계속 보게 될 것을 설명하였습니다.  
> 이제 배울 내용도 계속 보게 될 기본적인 기반 내용입니다.  
> 모든지 기본이 중요하니까 열심히 해야겠죠?


- - -
## 변수
> 프로그램의 기본

변수는 두가지의 뜻으로 설명 할 수 있을 것 같습니다  

코드 상에서는 값을 대입시켜 변화시킬 수 있는 요소라고 할 수 있지만  
메모리 상에서는 데이터를 담는 일정 크기의 공간이라는 의미도 가질 수 있습니다.  

여기서 메모리 상에서라고 설명하였을 때 '공간'이라고 설명하였는데  
중요한 내용은 아니고 "아 변수를 만들게 되면 메모리에 공간이 만들어지는구나!" 만 알고 있으면 됩니다.  

이제 코드를 작성해봅시다  

```cs
  int x;
```
> int -> 데이터 형식  
> x -> 변수의 이름  
> ; -> 문장의 끝  
> 변수를 만든다는 것을 **선언**이라고 부른다.  

보시다시피 가장 먼저 데이터 형식을 명시하고   
그 다음으로 변수의 이름을 명시힙니다.  
이렇게 문장을 작성하면 컴파일러는 int 형식에 맞는 메모리 공간을 부여하고  
x 라는 이름으로 사용할 수 있도록 준비합니다.

```cs
  x = 100;
```
> x -> 변수의 이름  
> = -> 대입 연산자  
> 100 -> 데이터  

이 코드가 실행되면 x 라는 이름을 가진 메모리 공간에 100이라는 데이터가 기록됩니다.

```cs
  int x = 100;
```
> 변수의 선언과 값 기록을 동시에 하는 것을 **초기화** 라고 부른다.

이 코드처럼 변수를 만드는 것과 데이터 기록을 동시에 할 수도 있습니다.  
이걸 초기화라고 부르기도 합니다.

밑 코드는 변수를 만드는 코드의 변환 입니다.
```cs
  int a, b, c;
```
> a, b, c 라는 변수를 한번에 여러개 선언

```cs
  int a = 10, b = 20, c = 50;
```
> a, b, c 라는 변수를 선언함과 동시에 데이터를 기록하는 것을 동시에 하는 코드

- - -
## 값 형식과 참조 형식
> 변수의 내부적인 구조알기

값 형식은 변수가 값을 담는 데이터 형식을 말하고  
참조 형식은 변수가 값 대신 값이 있는 곳의 위치를 담는 데이터 형식을 말합니다.  

아마 숙련된 개발자가 아니라면 이 문장을 보고 바로 이해하지 못할 것 입니다.

이걸 이해하기 위해서는 C#으로 작성한 코드가 사용하는 두 가지의 메모리 영역을 알아야 합니다.
첫번째가 스택(Stack)이고 두번째가 힙(Heap) 입니다.
값 형식과 관련있는건 스택이며 참조 형식과 관련 있는 것은 힙입니다

- - -
## 스택과 값 형식
> 스택에 대해 알아가보기

스택에 대해서 설명을 해가며 이해해봅시다.

스택은 책이 쌓인다는 것과 같은 구조를 가지고 있습니다.  
총 10개의 책이 쌓여 있다면 가장 밑의 책을 꺼내기 위해서는 총 9개의 책을 빼내고 그 작업을 할 수 있습니다.  
스택 메모리도 이와 똑같이 작동합니다.  

```cs
{ // 코드 시작
  int a = 100;
  int b = 200;
  int c = 300;
} // 코드 끝
```
> a, b, c 변수 선언하고 각각 100, 200, 300의 값을 저장
> 중괄호( '{', '}' ) 로 시작과 끝을 만들게 되면 그것을 코드 블럭이라고 부른다.

> 여기에 밑 문장의 설명을 돕는 이미지 만들기

이 코드블럭을 시작하면 a, b, c 순서로 쌓이고  
코드블럭이 끝나게 되면 c, b, a 순서로 데이터가 나가게 됩니다.

- - -
## 힙과 참조 형식
> 힙에 대해 알아보기

앞에서 본 스택의 구조를 보면 알다시피 자신이 사용한 데이터를 끝나면 확실히게 정리하는 메모리 구조입니다.  
반면에 힙 메모리 구조는 저장된 데이터를 수거하는 기능을 가지고 있지 않습니다.  

그래서 청소부 역할을 해주는 것이 따로 있는데  
그것이 가비지 컬렉터(Garbage Collector)입니다.  

가비지 컬렉터는 프로그램 뒤에서 지켜보며 힙에서 사용되지 않는 것이 있다면 그것을 쓰레기로 간주하고 수거해가는 기능을 합니다.

다시 참조로 돌아와서 설명하면  
참조 형식의 변수는 힙과 스택을 합께 이용하는데  
힙 영역에는 데이터를 저장하고  
스택 영역에는 데이터가 저장된 힙 메모리의 주소를 저장합니다.  

```cs
  object a = 10;
  object b = 30;
```
> object 가 뭐지 할 수 있는데 object는 참조 형식 변수라는 것만 알아두고 넘어갑시다.

이 코드가 실행되면  
스택에는 a와 b의 이름을 가진 변수에 힙 메모리의 주소가 저장되고  
힙에는 각각의 메모리 주소에 10과 30의 값이 저장됩니다.

코드가 끝나면 스택에 있던 메모리가 저장된 변수는 수거되고  
힙에 있던건 삭제가 되지 않다가 가비지 컬렉터가 쓰레기로 간주하고 수거해 갑니다.


- - -
## 기본 자료형

자료형이란 변수의 종류를 의미합니다. C#에서는 변수를 사용하기 전에 정수, 실수, 문자열 등 어떤 데이터를 저장 할 것인지 정의해주어야 합니다.  
기본자료형으로는 이것들이 있습니다.

![vyo](https://user-images.githubusercontent.com/70933806/175185874-1c6574c3-a066-4764-a51c-f06e8639ef9b.png)

표안에 있는 것들이 기본 자료형 입니다.

변수는 주로 정수, 실수, 문자, 문자열, 논리로 나뉘는데  
나누어보면 

```
정수 : byte, short, int, long  
실수 : float, double, decimal  
문자 : char  
문자열 : string  
논리 : bool  
```

이렇게 됩니다.
다만 표를 잘 보면 앞에 's' 와 'u' 가 붙은 것들은 써놓지 않았는데  
설명부터하면 's' 는 'signed' 라는 단어의 줄임말로 부호가 있다는 의미이며,  
'u' 는 'unsigned'로 부호가 없다는 뜻 입니다.  

그래서 sbyte는 -128 부터 127까지 음수부터 양수를 담을 수 있고  
ushort는 0부터 65535까지 양수만 담을 수 있습니다.  

다시 돌아와서 이게 뭐하는 자료형인지 설명하도록 하겠습니다.

```
정수 - 123, 5432, 1023  
실수 - 0.123, 123.132   
문자 - 'a', '1', '~'  
문자열 - "Hello World", "겜마고"  
논리 - true, false  
```

아마 대강 보면 바로 이해가 가실겁니다.  
근데 여기서 드는 의문이 정수와 실수에는 왜 같은 것인데도 불구하고 여러개의 자료형이 있는지인데,  

그 이유는 크기 때문입니다.  
우리가 0부터 10까지의 수만 사용한다면 굳이 9,223,372,036,854,775,808까지 저장할 수 있는 long보다는 byte를 사용해서 메모리를 절약 할 수 있겠죠?  

- - -
## 조건문
## 반복문
> 어째서 두 챕터가 한 곳에 있는걸까

https://docs.microsoft.com/ko-kr/dotnet/csharp/tour-of-csharp/tutorials/branches-and-loops?tutorial-step=1

이 링크에서 조건문과 반복문에 대한 내용을 자세히 배울 수 있습니다.  
참고해서 해주세요 절대 일정이 밀려서 이 링크를 제시하는 것이 아닙니다.  

