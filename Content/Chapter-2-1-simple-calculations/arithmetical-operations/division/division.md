### Деление на числа (оператор **`/`**)

Делението на числа се извършва с оператора **`/`**. Той работи различно при цели и при дробни числа.
* Когато делим две цели числа, се извършва **целочислено деление** и полученият резултат е цяло число с отрязана дробна част. Например 11 / 3 = 3.
* Когато делим две числа, от които поне едното е дробно, се извършва **дробно деление** и полученият резултат е дробно число, както в математиката. Например 11 / 4.0 = 2.75. При невъзможност за точно разделяне, резултатът се закръгля, например 11.0 / 3 = 3.66666666666667.
* Целочисленото **деление на 0** предизвиква **грешка** по време на изпълнение (runtime exception).
* Дробното **деление на 0** не предизвиква грешка, а резултатът е **+/- безкрайност** или специалната стойност **NaN**. Например 5 / 0.0 = &#8734;.

Ето няколко примера за използване на оператора за делене:

```csharp
var a = 25;
var i = a / 4;      // извършваме т.нар. целочислено деление:
                    // резултатът от тази операция ще бъде 6 – дробната част се отрязва, 
                    // тъй като извършваме деление с цели числа
var f = a / 4.0;    // 6.25 – дробно деление. Изрично сме указали числото 4 да се интерпретира
                    // като дробно, като сме добавили десетичната точка, следвана от нула
var error = a / 0;  // Грешка: целочислено деление на 0
```
