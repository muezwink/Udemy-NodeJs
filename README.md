# 자바스크립트 개요
https://developer.mozilla.org/en-US/docs/Learn/JavaScript
https://academind.com/tutorialsf

# 핵심 구문 복습
01-core-js-syntax.zip  
[JavaScript from Scratch-자바스크립트 처음부터 배우기](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)  
[Various JavaScript Beginner Resources-다양한 자바스크립트 초보자 리소스](https://academind.com/tutorials/)  
[Primitive vs Reference Types-프리미티브 유형과 참조 유형](https://academind.com/tutorials/)  

# let & const
02-let-and-const.zip

# 화살표 함수의 이해
03-arrow-functions.zip
[Arrow Functions and "this"](https://academind.com/tutorials/)  

# 개체, 속성 및 메서드 작업
[Primitive vs Reference Types](https://academind.com/tutorials/reference-vs-primitive-values)

# 배열과 배열 메서드
[Available Array Properties & Methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array#)

# 배역, 객체 및 참조 유형
[
현대의 JavaScript에는  
반드시 알아야 하는 두 개의 연산자가 있고  
강의에서도 계속 사용할 예정입니다  
바로 레스트(Rest)와 스프레드(Spread) 연산자입니다, 구체적으로 들어가서  
레스트 연산자는 꽤 자주 사용하게 될 것입니다  
새로운 hobby를 추가할 때마다 기존의 배열을  
편집하고 싶지 않다고 해보겠습니다  
대신 기존 값과 새로운 값이 모두 포함된 새로운 배열을 만들고 싶다고 해보겠습니다  
이는 불변성이라 불리며 꽤 자주 등장하는 패턴입니다  
기존의 값을 절대 편집하지 않고  
사본에 변경된 값을 더한 배열로 대체하는 방식입니다  
이 강의에서 자주 사용하게 될 패턴입니다  
복사해서 편집함으로 오류를 피할 수 있고  
기존 객체를 편집하지 않음으로써  
코드를 읽어올 수 없게 되는 일을 방지할 수 있습니다  
배열을 복사하려면 여기 copiedArray를 생성합니다  
몇 가지 기법이 있습니다  
하나는 슬라이스 연산자를 사용하는 것으로  
여기에 copiedArray를 입력하고 node play.js를 실행하면 Sports와 Cooking이 보입니다  
복사되었음을 볼 수 있습니다  
slice는 배열을 복사합니다  
인수를 입력해서 복사하길 원하는 원소의 범위를 제한할 수 있습니다  
인수가 없으면 배열 전체가 복사됩니다  
slice 외에 다른 기법도 있습니다  
대괄호로 새로운 배열을 만들고  
hobbies를 추가해도 됩니다  
이를 실행하면 어떻게 될까요?  
콘솔에 무엇이 표시되는지 보겠습니다  
Enter를 누르면 사본처럼 보입니다 그러나 실제로는 배열 안에  
또 다른 배열이 있는 겁니다  
외부 배열에 하나의 원소만이 있고 그 원소가 바로 내부 배열입니다  
따라서 사본이 아니라 첫 원소가 기존의 배열인 새로운 배열일 뿐입니다  
이는 사본이 아니라 완전히 동일한 객체를 의미합니다  
따라서 우리가 만든 것은  
중첩 배열로 이는 원하던 작업이 아닙니다  
여기서 사용 가능한 스프레드 연산자는 배열 또는  
객체 앞에 추가하는 점 세 개입니다  
이 점 세 개는 +나 -와 같은 연산자로  
연산자 뒤에 오는  
배열이나 객체를 받아서  
원소나 속성을 끄집어냅니다  
따라서 배열의 원소나 객체의 속성을  
스프레드 연산자 주위에 있는 대상에 추가합니다  
이 경우에는 스프레드 연산자에 대괄호가 씌워져 있으므로  
기존의 배열에서 끄집어낸 모든 원소를  
새로운 배열에 추가해 줍니다  
따라서 이 파일을 저장하고 다시 실행하면  
기존 접근법의 중첩 배열이 있던 곳에  
중첩 배열이 없어졌습니다  
대신 배열 하나가 있고 이 배열은 기존 배열의 사본입니다  
스프레드 연산자로 원소를 끄집어내서  
새로운 배열에 하나씩 추가했기 때문입니다  
기존의 배열이나 객체에 이러한 작업을 많이 하게 될 것입니다  
객체에서도 같은 방식으로 작동합니다  
중괄호로 copiedPerson을 만들고 스프레드 연산자를  
점 세 개로 입력하고 기존의 Person을 입력합니다  
이제 copiedPerson을 console.log 하고  
이 파일을 다시 실행하면  
여기에 person의 사본이 나타납니다 객체의 원소를 모두 추출해서  
새로운 객체에 추가했기 때문입니다  
이는 객체와 배열 모두에 적용 가능합니다 그리고 이 구문을  
이 강의에서 자주 사용하겠습니다  
이게 바로 스프레드 연산자입니다  
레스트 연산자도 언급했는데 레스트 연산자는 정 반대입니다  
toArray라는 이름의 화살표 함수가 있다고 해보겠습니다  
arg1, arg2, arg3 인수가 있습니다  
이 인수들을 포함한 배열을 반환하도록 하고 싶습니다  
여기에 등호를 추가해 줍니다  
이 인수들을 포함한 배열을 반환하게 하고자 합니다  
return 대괄호를 입력하고 첫 번째 원소는 arg1,  
두 번째 원소는 arg2, 세 번째 원소는 arg3로 하면 됩니다  
이제 console.log (toArray)를 입력하고  
1, 2, 3,을 각각 인수로 함수에 입력한 다음  
play.js를 실행하면 1, 2, 3 세 개의 원소가 포함된 배열이 보입니다  
제대로 됐습니다 그러나 이는 전혀 유연하지 않습니다  
네 개의 인수를 입력하고 싶다면  
이렇게 호출할 수도 있습니다  
JavaScript는 이를 허용합니다  
그러나 세 개의 인수만으로 작업했기 때문에 추가되지는 않습니다  
이럴 때 레스트 연산자를 활용할 수 있습니다  
... 뒤에 args를 입력합니다  
이렇게 하면 개수에 관계없이  
모든 인수를 가지고 와서  
하나의 배열로 나타냅니다  
여기서 args는 배열이 되며 이를 반환하게 할 수 있습니다  
이제 toArray에 4개의 인수를  
입력하고 다시 실행하면 이제 4개의 인수가 있는  
배열을 얻을 수 있습니다 레스트 연산자는 스프레드 연산자처럼  
세 개의 점으로 되어있으며 사용하는 위치에 따라 정의가 달라집니다  
배열이나 객체에서 원소나 속성을 추출하는 데 사용한다면  
스프레드 연산자입니다  
인수 목록이나 함수에서  
여러 인수를 하나의 배열로 묶는데 사용한다면  
레스트 연산자입니다  
구문으로 보면 동일한 연산자이지만  
사용하는 위치에 따라 이름이 달라집니다  
이 구문은 강의에서 자주 사용하지는 않겠지만 그래도 알아두면 좋습니다  
그러나 원소 또는 속성 추출은 반드시 이해해야 합니다  
이 강의 전반에 걸쳐서  
자주 사용할 구문이기 때문입니다
]

# 스프레드(Spread) 및 레스트(Rest) 연산자의 이해
[차이점](https://chat.openai.com/c/4851a6d4-70ee-4c6f-b7ce-03c93a7efd7b)  

# Destructuring (구조분해)
[배열과 객체의 구조분해, 객체를 인자로 받는 함수에서의 구조분해](https://chat.openai.com/c/2fbe5a80-9873-40cd-85eb-05e1efe6cc49)

# 비동기 코드와 프로미스
[
다시 play.js 파일을 지웠습니다
빠르게 복습 모듈을 마치고 다른 핵심 개념인
비동기화 코드를 다루는 방법을 배우기 위해서입니다
이를 위해 먼저 비동기화 코드가 무엇인지부터 이해해야 합니다
Node.js에 구축되어 있는 함수인 타이머 종료 시간을 설정한다고 가정합시다
이 경우 일정 시간 이후 실행 또는 종료되는 함수를 정의하게 됩니다
저는 화살표 함수를 사용하지만
이름이 지정된 함수 등 다른 함수를 사용해도 좋습니다
두 번째 인수는 타이머입니다
2초라고 합시다 밀리초로 표현해야 해서
2초라면 2000 밀리초가 되겠죠
이 안에 간단하게 타이머가 끝났다고 적겠습니다
이제 이 파일을 2초 동안 실행하게 되면
아무 일도 일어나지 않고 타이머가 끝난 것을 볼 수 있습니다
이게 바로 비동기화 코드로 즉시 끝나지 않기 때문에
1 밀리초를 입력했더라도 마찬가지로 비동기화 코드에 해당합니다
아무리 빠르다고 해도 즉시 발생하는 것은 아닙니다
코드 구간에서 예를 들면 console.log
('Hello!'), 그리고 console.log('Hi!')가 있을 때
이 스니펫은 비동기화 코드로 각자가 끝난 뒤 곧바로 실행되지만
기술적으로는 실행되기까지 시간이 좀 소요될 텐데, 하드웨어를 제외하고는
딜레이가 존재하지 않으므로 동기화 코드이고
이것이 비동기화 코드로 즉시 실행되거나 끝나지 않고
짧긴 해도 시간이 소요됐기 때문입니다 이 파일을 이렇게 실행하면
종료되기 전에 Hello!와 Hi!가 아주 짧게나마 나타납니다
왜냐하면 Node.js와 JavaScript는 일반적으로
코드 실행이 종료될 때까지는 이를 멈추지 않기 때문입니다
여기에서는 콜백 함수라고 하는 함수를 인식할 것입니다
즉 함수는 나중에 실행될 것입니다
추후 완료된 이후에 답신하게 됩니다
따라서 여기에서 타이머가 종료된 뒤에 이걸 인지하게 되며
우리는 곧바로 다음 줄로 이동해서
모든 동기화 코드를 실행하고
이게 종료된 뒤에 비동기화 코드가 실행됩니다
그래서 코드에서 Timer is done!이 먼저 출력됐음에도
Hello!와 Hi!를 먼저 보게 되는 것입니다
JavaScript와 특히 Node에서 이 개념은 반드시 이해해 둬야 합니다
정말 중요하기 때문에 강의 전반에 걸쳐 다시 언급하도록 하겠습니다
이제 이걸로 작업하면서
뚜렷하게 하기 위해 2초로 이 값을 올리면
동기화 코드가 실행되는 것을 다시 볼 수 있고
2초가 지난 뒤에 이 코드가 실행됩니다
비동기화 코드로 작업할 때는 이를 다루는 기법들이 여러 가지 있습니다
콜백 함수는 그중 가장 오래된 함수이며
특히 Node.js에서 자주 보게 될 것입니다
잘못된 건 전혀 아닙니다
그러나 몇 가지 의존성 비동기 작업의 경우 문제에 직면하게 됩니다
여기에서는 타이머를 설정하고 다른 함수 생성을 위해
fetchData라고 하겠습니다
여기에도 타이머를 설정하는데
데이터를 가져오게 되는 데이터베이스 같은 걸
설정하고 싶지 않아, 강의를 진행하면서 다루게 되니 걱정 마세요
여기에 또 다른 타이머는 1.5초 정도로 하겠습니다
그리고 여기 fetchData에서 저는 이 내부 타이머가 끝났을 때
뭔가를 실행시킬 필요가 있습니다
여기서 저는 callback이라고 지정할 인수를 입력합니다
이 인수는 타이머가 끝난 뒤에 제가 내부 함수로 호출할 함수이기 때문입니다
여기에서 Done!이라는 값을 입력하고
fetchData를 사용하는 장소가 여기
setTime 내부라고 하고 호출하겠습니다
이렇게 fetchData를 호출합니다 여기에서 또 다른 콜백이 필요합니다
실행하게 되면 여기에서 함수를 콜백 하기 위해
텍스트가 전달되어 텍스트를 입력하고
그 텍스트를 console.log 할 수 있죠
조금 혼란스러울 수 있는데
저는 저만의 함수를 생성하는 중으로, 콜백을 받음으로써
이 내부 타이머가 다른 곳에서 완료되었을 때
실행되는 함수를 정의할 수 있습니다
그러니까 여기에서 이 함수는 콜백으로 전달되는 것입니다
그리고 여기서 그 함수를 실행합니다
이제 이걸 저장하고 실행하면
2초가 지난 뒤에 Timer is done!,
그리고 다시 1.5초 후에 Done!이 보입니다
만약 중첩된 비동기화 호출이 여기에서처럼 몇 개 존재하는 경우
우리는 콜백 시점에서 점점 더 깊게 들어가게 됩니다
그렇기 때문에 프로미스(Promise)라는 기능을 Node.js에서 사용할 수 있습니다
이미 프로미스가 사용된 제3자 패키지를 자주 사용할 것입니다
따라서 여기에서 보여드릴 구문은 직접 작성할 일은 거의 없습니다
내부 패키지가 진행하게 되겠죠
그래도 알아두면 좋습니다 fetchData 함수 내부에
프로미스를 생성한다고 해봅시다
상수 또는 변수로 저장하고
JavaScript 내부에서 생성자를 기반으로
새로운 객체를 생성하는 new 키워드를 사용합니다
만약 생성자 함수의 의미가 전혀 와닿지 않는다면
JavaScript에 관련된 기본 개요 자료를 찾아보세요
생성자 함수는 JavaScript의 핵심 기능이기 때문입니다
여기에서는 JavaScript와 Node.js
내부에 구축된 프로미스 생성자 함수를 사용합니다
이후 resolve와 reject라는 두 가지 인수를 콜백하게 되는데
이름은 자유롭게 붙여도 되고 어쨌든 두 함수가 들어옵니다
첫 번째 함수는 프로미스를 성공적으로 완료하여
성공적으로 해결합니다
두 번째 함수는 거부하게 되는데 예를 들면 에러를 표시하는 거죠
다음으로 비동기화 코드를 안으로 이동시킬 수 있습니다
다시 강조하지만 이건 직접 작성할 일은 거의 없습니다
대부분의 패키지들이 이미 알아서 진행해 주고
완료된 프로미스를 전달하여 배후에서
전부 다 해결해 주지만 지금은 수동으로 진행해 보는 것이죠
콜백 내부에 함수가 있는데
안타깝게도 setTimeout이 프로미스 API를 제공하지 않아
여기에도 콜백을 사용해야 하지만
이제 더 이상 우리가 얻게 되는 콜백 함수를 사용할 수 없고
더 이상 여기에서는 인수를 얻거나 데이터를 가져올 수 없습니다
대신 resolve('Done!')을 입력하여 성공적으로 결괏값을
반환합니다 이제 fetchData에서
프로미스를 정의한 뒤에는 반환하기만 하면 됩니다
이건 동기화 코드라는 걸 기억해 주세요
이제 이건 프로미스 내부의 코드가 실행되기 전에
프로미스가 생성된 직후 반환될 텐데,
이 함수를 호출하고 이 타이머의 Done!이 완료되고 얼마 후
일어날 일입니다
이제 프로미스를 여기로 반환하고 fetchData를 호출하는 자리에
더 이상 콜백을 전달하지는 않지만 프로미스 상에서
호출할 수 있는 then을 사용하고 프로미스를 반환할 수 있습니다
이건 단순히 콜백 함수를 여기에 정의해서
프로미스가 해결된 뒤에 실행되도록 합니다
그런 프로미스가 여러 개 있을 때 장점은 뭐가 있을까요?
여기에 fetchData를 다시 호출했다면
이런 식으로 then을 사용할 필요가 없습니다
이 경우 다시 콜백이 중첩되겠죠
대신 프로미스 내부에 블록이 프로미스의 일부인 경우
간단히 새로운 프로미스를 반환하고
다음 then 블록을 이전 블록 다음에 추가할 수 있습니다
이렇게 하면 then 블록이 연쇄적으로 구성되어
첫 번째 프로미스 다음에는 이 블록이 호출되고
then 블록 내부에서 다른 프로미스를 반환하게 됩니다
프로미스를 전달하지 않는다고 해도 then 블록은 이걸 반환하는 대신
즉시 해결되는 프로미스로 전환하게 됩니다
그리고 여기 이 프로미스에 관련된 다른 then 블록을 추가하면
무한히 중첩된 콜백을 두는 것보다 훨씬 읽기 편합니다
이걸 실행해 보면 Hello!, Hi!, Timer is done!이 보입니다
Done!은 두 번 나타나는데
fetchData를 두 번 호출하기 때문입니다
처음 접하게 되면 정리하기에 좀 어려울 수 있습니다
이 강의를 진행하면서 계속 다시 사용하면
좀 더 명확해질 것입니다
재차 말씀드리지만 이 코드는 직접 작성할 일이 거의 없지만
우리의 비동기화 코드를 더 잘 관리할 수 있는 핵심 개념입니다
이를 관리하는 다른 방법이 존재하는데
현대 JavaScript에서는 async, await와 특수
키워드를 사용할 수 있으며 강의 후반부에서
따로 설명드리겠습니다
이 구문보다 더 복잡할 수 있어 여기에서 소개해 드리고 싶진 않습니다
한 번에 너무 많은 새 기능을 소개해 드리고
싶지는 않으므로 이것 하나만 하겠습니다
하지만 비동기 코드는 이해해 두셔야 합니다
이 시점에 완전히 이해하고 계시지 않아도 괜찮습니다
강의 내내 자주 등장할 것입니다
왜냐하면 Node.js에는 여러 비동기화 이벤트가 있으며
있으며 저도 여러 번 설명할 것이기 때문입니다
프로미스도 다시 설명하니
현재로서는 최소한 한 번 보고
작동 방식과 활용 방법을 이해할 기회를 드리고 싶습니다
]

# 템플릿 리터럴 
[
템플릿 리터럴(Template literals)이라는 기능을 종종 사용하게 될 거예요.  https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals
문자열을 작성하는 다른 방법입니다.
큰따옴표나 작은따옴표를 사용해
'A String'
혹은
"Another string"
와 같은 방식으로 표현하거나,
백틱(`)을 사용해
`Another way of writing strings`
와 같은 방식으로 표현합니다.
왜 문자열을 이런 방식으로 표현할까요?
이 구문을 사용하면, 문자열에 다양하게 데이터를 추가할 수 있어요.
const name = "Max";
const age = 29;
console.log(`My name is ${name} and I am ${age} years old.`);
처럼요.
기존의 문자열 결합 방식보다 짧고 읽기 쉽습니다.
const name = "Max";
const age = 29;
console.log("My name is " + name + " and I am " + age + " years old.");
와 비교해서 말이죠.
]

# 유용한 자료 및 링크
[MDN JavaScript 튜토리얼](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)
[Academind JS 자료](https://academind.com/learn/javascript)

# Node 서버 생성
[nodejs의 코어모듈과 라이브러리](https://chat.openai.com/c/0b4047bc-4a2b-4fa6-a815-78a5d4d99466)

# 요청과 응답 헤더
[요청과 응답 헤더](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers)

# 라우터 요청

# 이벤트 기반 코드 실행의 이해

# 블로킹 및 논블로킹 코드
[
그럼 여기 이 writeFilesSync 라인은 뭐가 문제일까요?  
Sync 키워드가 문제 있습니다  
앞서 말씀드렸듯이 writeFile 메서드도 존재하지만  
writeFileSync를 사용하였습니다 여기에서 sync는  
동기화를 의미합니다 그리고 이것은 이 파일이 생성되기 전까지  
코드 실행을 막는 특별한 메서드입니다  
이 파일들을 작업하는 데에는 두 가지 모드가 존재하는데  
파일이 완료될 때까지 코드의 다음 라인이 실행되지 않도록 하는  
동기화 모드가 있습니다  
우리가 입력하는 이 짧은 텍스트의 경우 알아차리지도 못할 정도로 아주 빠르지만  
수백 메가바이트 이상의 큰 파일에서  
이 방법을 적용함으로써  
읽거나 복사하는 등의 상황에서 코드 실행을 막는 경우  
다음 줄과 다른 모든 코드가  
파일 운영이 완료될 때까지 실행을 멈출 것이며  
다른 유저들이 보내어 새로 유입되는 요청들도  
파일 운영이 끝나기 전까지는 취급되지 않을 것입니다  
그런 건 원하지 않을 테니 여기선 해당 구문을 사용하지 않겠습니다  
매우 짧은 파일 운영만을 진행하는 경우  
사용할 수는 있겠지만 그렇다 하더라도 이 파일 쓰기 방법을  
사용하는 편이 더 나은데, 경로와 데이터를 받아들일 뿐만 아니라  
세 번째 인수인 콜백까지도  
포함하기 때문이며  
따라서 완료된 뒤에 실행되어야 하는 함수에 해당합니다  
그래서 서버 생성 때와 마찬가지로 Node.js는 암묵적으로  
이벤트 리스너를 등록시킵니다  
여기에서 다른 함수를 넘기고 이 콜백은 오류 객체를 전달받는데  
오류가 발생하지 않았다면 공란으로 남아있을 테지만  
권한 누락을 비롯한 어떤 오류가 발생한 경우라면  
여기로 가져오게 되며  
다른 종류의 응답, 즉 사용자에게  
오류가 발생했음을 나타내는 오류 응답 등을 반환하고  
그렇지 않다면 정상 응답을 반환하는 방식으로 처리할 수 있습니다  
지금은 오류에 대해 다루지 않을 예정이고 딱히 뭔가 잘못될 부분도 없습니다  
물론 강의를 좀 더 진행한 뒤에는 오류에 대해서도 살펴보도록 하겠습니다  
이 응답은 파일 작업이 완료된 경우에만 전송되어야 하기 때문에  
일반 응답 코드를 거기로 옮기겠습니다  
이게 요청에 따라 결국 수행하려는 작업이기 때문입니다  
이제 이벤트 리스너와 함께 요청을 파싱 하는 것이 끝난 뒤  
실행하게 될 메서드 내지는 함수를 확보하게 되었으며  
추후 언젠가 실행될 해당 함수 내부에도  
또 다른 이벤트 리스너가 있고 여기 이렇게 중첩된 함수는  
우리가 파일을 기록하는 과정이 끝난 뒤에 실행될 것이며  
이러한 과정은 Node.js에서 상당히 표준적입니다  
이벤트 드리븐 아키텍처에서는  
Node.js에게 작업을 진행하도록 지시하며  
이후 Node.js가 해당 프로세스를  
멀티 스레딩을 사용하는 운영체제에 전달하며  
이벤트 콜백을 파악하기 위해  
이벤트 루프를 계속하면서  
코드 실행을 막지 않도록 그런 작은 조치들을 발송하고  
운영체제에서 작업이 끝난 뒤에는  
항상 복귀하는 식의 구조를 지닙니다  
이게 바로 Node.js의 구조이며 그토록 뛰어난 성능을 발휘하는 이유로  
여러분의 코드를 절대 막지 않고 서버를 막는 일도 없으며  
단지 계속해서 운영체제에게 작업들을 할당하고  
완료된 뒤에는 돌아와서 콜백에서  
응답을 전달하는 등의 작업을 진행하는데 이는 헤더 몇 개만  
진행하면 끝나는 작업이므로 전체 운영을 막는 일이 없습니다  
충분히 이해하셨길 바라고  
이제 서버를 종료 후 다시 시작하겠습니다  
노드 앱을 다시 실행한 뒤 /뒤에는 다 지우고요  
여기 Hello again을 입력해서 전송해 보겠습니다  
message.text를 다시 보면 again이 추가 문자로 연결되어 있지만  
지금은 여기에 대해 걱정할 필요가 없습니다  
이렇게 writeFile도 작동하는 걸 확인해 봤는데  
Node.js의 비동기적 특성으로 인해 이런 방법으로 사용해야 합니다  
이 부분은 Node.js의 핵심 개념이고  
분명히 이해해야 하는 부분입니다  
핵심적인 기본 사항들을 다루는 걸로 이 모듈을 마무리하고  
이제 좀 더 쉬운 방법으로 넘어가서  
이런 핵심적인 세부 코드를 우리가 직접 쓰는 일 없이  
더 간편하게 작성해 보도록 합시다  
하지만 이 부분의 작동 원리를 이해하는 것은 정말로 중요합니다      
]

# Node 모듈 시스템 사용
[
이제 이번 모듈을 마무리할 시간입니다
마치기 전에
코드를 조금 고쳐볼까요
한 파일만 해도 이렇게 많은 코드가 있는데
보통은 여러 파일을 작업하게 될 거예요
url 확인 등의 작업을 하는 라우팅 로직을 포함한
새 파일을 만들어볼까요
routes.js라는 새 파일을 생성할게요
이름은 마음대로 지으셔도 됩니다
그러면 이런 아이콘이 뜨는데
보통 JavaScript 파일입니다
routes.js 파일에
if문과 기본 응답 코드를 넣기 위해
app.js 파일에서 잘라내서
깔끔한 파일로 남긴 다음 routes.js에 붙여 넣습니다
그중에 if문은
아마 다른 방법을 사용해야 할 거예요
하지만 코드는 옮겨졌으니
이제 app.js에 필요하지 않은 파일 시스템은 제거합니다
http는 아직 필요하지만
url과 method는 필요하지 않으니
지운 다음 routes.js로 넘어가
가장 위에 fs를 추가한 상태에서
시작합시다
이제 routes.js 파일에 뭘 해야 할까요
app.js를 routes.js로 연결할 수 있어야겠죠
들어오는 요청을 routes.js 파일로
보낼 수 있어야 하니까요
새로운 함수로
requestHandler 함수를 생성해
req, res를 인수로 가지면
http.createServer 함수를 대체하게 됩니다
혹은 ES6 함수를
상수 requestHandler에 저장할 수 있죠
처음 보는 구문이라면 낯설게 느낄 수 있는데
근본적으로
상수에 저장하는 익명의 화살표 함수이며
함수의 이름은 requestHandler입니다
이제 req, res를 넣은 후
아래에 있는 모든 코드를 함수로 옮겨야 합니다
코드가 요청 및 응답 객체를 사용하기 때문에
인수가 같은 이름을 사용하도록 만들면
로컬 변수로 사용 가능하게 되는 거죠
url과 method도 사용하기 때문에
req.url과 req.method의 데이터를
다시 상수로 추가해야 합니다
이제 핸들러를 내보내기만 하면 되는데요
불러올 때는 require 구문을 사용했다면
내보낼 때는 어떻게 해야 할까요
내보내기를 하는 두 가지 방법이 있습니다
첫 번째 방법은 가장 아래에
module.exports를 추가하는 겁니다
Node.js에 의해 전역으로 노출된
키워드 혹은 객체로 내보내기 속성이 있어서
requestHandler 등의 값을 지정하면
다음과 같은 함수를 가진 requestHandler 상수가
module.exports에 저장됩니다
노출된 전역 객체이기 때문에 Node.js가 처리할 수 있죠
이제 require로 routes.js 파일을 불러오면
Nodes.js가 module.exports를 찾아
등록된 것이 있는지 보는데요
우리는 module.exports에
requestHandler를 등록했죠
여러 키-값 쌍을 가진 JavaScript 객체를 추가해도 되고
원하는 대로 추가할 수 있는데
저는 이 함수를 등록했어요
이제 app.js로 돌아가
원하는 대로 상수 이름 routes를 입력하고
require을 통해 불러옵니다
글로벌 모듈이 아니기 때문에 routes만 입력하지 않고
./로 로컬 경로를 추가하는데
대신 끝에 .js는 생략해도
Node.js가 자동으로 붙일 거예요
물론 직접 .js를 붙여도 되지만 저는 ./routes만 입력할게요
또 상단의 코어 모듈과 분리해서
사용자 지정 파일임을 분명히 하겠습니다
그럼 Node.js가 app.js와 같은 폴더에서
routes.js 파일을 찾아서
module.exports에 무엇이 등록되어 있는지 볼 겁니다
이때 requestHandler 메서드를 내보내면
routes를 통해 사용할 수 있게 됩니다
파일에서 내보내는 모든 것들을
routes 상수로 지정했기 때문이죠
routes 상수가 이 함수를 갖고 있으므로
여기서 핸들러로 사용할 수 있는 거예요
routes를 입력한 후 실행하지 말고
괄호도 넣지 않은 채 이름만 입력해서
들어오는 요청에 대해 routes에 저장된 함수를
실행하라고 알려줍니다
저장한 후에 서버를 재시작하고
이 페이지를 재로딩해도 문제없고
Test를 발송해 봐도 문제없네요
message.text에 Test가 저장됐습니다
이렇게 코드를 두 파일로 나눴습니다
깔끔한 app.js 파일은 서버를 가동하는
중요한 역할을 하고
불러오기와 내보내기를 통해 routes.js 파일로 연결해요
requestHandler의 함수를 내보냈죠
바로 이런 원리입니다
Node.js 모듈 시스템에서 한 가지 중요한 점은
파일 내용의 캐시가 저장되고
외부에서 수정할 수 없다는 겁니다
만약 routes를 객체로 정의하고
새로운 속성을 추가하려고 하면
원본 파일을 조작할 수 없어요
즉 잠금 되어 외부가 접근할 수 없기 때문에
외부에서 읽을 수 있는 내용만 내보내기 할 수 있는 겁니다
내보내는 함수가
내부적으로 변경 사항을 만들 수는 있지만
지금 당장 너무 깊게 들어가지 않고
강의를 진행하면서 차차 배워보겠습니다
지금 상태에서 module.exports 대신에
사용할 수 있는 구문이 하나 더 있어요
가끔 여러 내용을 한꺼번에 내보내기 하는 경우
객체로 handler 키워드를 입력하면
requestHandler 함수와 같고
someText를 입력하고
여기서는 Some hard coded text라고
입력하면 두 가지를 내보낼 때
둘을 그룹화하거나 분리하면서도
하나의 내보내기만 관리할 수 있게 됩니다
그러면 app.js에서 routes는
함수가 아닌 객체가 되는 거죠
그럼 여기서 handler 속성에 접근해야 하는데
이 속성은 사용하고자 하는 함수를 참조하고 있죠
아니면 console.log로
routes.someText를 출력할 수도 있습니다
이렇게 하면 하나의 파일에서 여러 내보내기를 할 수 있고
console.log로 인해 출력된 Some hard coded text가 보이는데
기능은 예전과 같습니다
이 코드 외에도 여러 가지를 내보내는
다른 방법은
module.exports.handler = requestHandler나
module.exports.someText = 'Some hard coded text'입니다
달라 보일 수도 있지만
아직 하나의 exports
즉 모든 내보내기를 묶는 module.exports가 있고
handler나 someText 속성을 지정했기 때문에
바로 이 코드와 똑같습니다
이제 저장한 후에 서버를 재시작하면
Some hard coded text가 출력되고
무작위로 입력해 제출하면 문제없이 작동되네요
마지막으로 이 구문에는 단축키가 있는데요
module를 생략하고 exports만 입력해도 됩니다
JavaScript 자체가 아니라
Node.js에 의해 특별히 지정된 단축키예요
이제 여러 개의 내보내기를 하나의 내보내기로 합쳤으니
다시 실행해 보면
역시 Terminal에는 Some hard coded text가 보이고
Some last value를 보내면
문제없이 작동되고
message.text에 남습니다
이렇게 여러 개의 파일을 연결해 봤습니다
module.exports = requestHandler라는
하나의 함수를 내보내는 것이
첫 번째 방법이었고요
앞에 슬래시 두 개를 붙여 코멘트로 만들어 둘게요
혹은 객체에 대한 module.exports로
여러 개를 합치거나
module.exports.handler = requestHandler나
module.exports.someText = 'Some text'를 사용하는데
아래에 있는 단축키와 같고
Node.js가 지원하는 단축키였죠
여기까지 불러오기 및 내보내기와
모듈 시스템의 원리에 대해 배웠습니다
강의를 진행하면서 많은 파일을 다룰 예정이기 때문에
꼭 이해하고 넘어가는 것이 중요합니다
그럼 이제 이번 모듈을 마무리하도록 합시다    
]