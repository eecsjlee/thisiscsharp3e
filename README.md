# 이것이 C#이다 3E
  
## 개발환경
Visual Studio 2022(Community)  
.NET 8.0  
C# 12
  
## 참고자료
https://github.com/sean-lab/ThisisCSharp3E  
https://learn.microsoft.com/ko-kr/dotnet/csharp/tour-of-csharp/  
https://github.com/DevExpress-Examples  
https://github.com/microsoft/WPF-Samples  

## 05 코드의 흐름 제어하기

### 매소드
Console.WriteLine("Hello World")  
Console.ReadLine()  
Convert.ToInt32(input)  
  
## 06 메소드로 코드 간추리기

### 메소드란?
C와 C++ 언어에서는 함수라 불렀다.

```csharp
class Calculator
{
    // 두 정수를 더하는 메소드
    static int Add(int a, int b)
    {
        return a + b;
    }

    // 문자열을 출력하는 메소드 (반환값이 없음)
    static void PrintMessage(string message)
    {
        Console.WriteLine(message);
    }

    // 메인 메소드 (프로그램 실행 시작점)
    static void Main(string[] args)
    {
        int result = Add(5, 3);
        PrintMessage("두 수의 합은 " + result + "입니다.");
    }
}
```

### 한정자
|구분|한정자|의미|
|:---:|:---:|:---:|
|접근 한정자|public, private, protected, internal|멤버의 접근 범위를 정의합니다.|
|정적 한정자|static|클래스 단위로 관리되는 멤버를 나타냅니다.|
|기타 한정자|abstract, virtual, override, sealed, readonly, const 등|멤버의 특성을 정의합니다.|

