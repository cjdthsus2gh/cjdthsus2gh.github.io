


컴파일러 수업을 들으면서 기억해 둘만한 것들을 적어두려고 한다.

## Language Processors의 역할

C나 C++, Java 같은 고급 언어들의 소스 코드를
**Semantically-equivalent** 한 target code 로 번역한다. 
컴퓨터과학에선 서로 다른 두 언어의 이 Semantically-equivalence 의미상의로 동등
에러 / 버그 감지

## Compilation  /  Interpretation

 
-프로그램을 실행하기 전에 컴파일을 하느냐, 한줄 한줄 내려가면서 실시간으로 하느냐의 차이

-또한 컴파일한 결과물이 프로그램이냐, 명령어와 같은 코드냐의 차이

-실행시간 
	컴파일러가 유리 (왜?)
-안정성 / 이식성
	특정 하드웨어에서만 실행 가능한 target code를 통째로 만들어내는 컴파일러보다 인터프리터가 유리
-디버깅 / 개발
	에러의 원인을 쉽게 찾을 수 있는 인터프리터가 유리

## + Hyblid Compilers
컴파일러와 인터프리터를 합친 새로운 모델. 빠른 실행시간 & 높은 이식성을 갖고 있음.

컴파일 결과로 Intermidiate Program ( e. g. **ByteCode** )생성
JVM 같은 거라고 보면 될듯?

## 일반적인 language-processing system 

Preprocessor -> Compiler -> Assembler -> Linker
*기계어와 Linker의 역할에 대해

좋은 컴파일러는 1. 정확성 2. 성능향상성 3. 컴파일 시간 면에서 우수해야 한다.

### Fortran Language ??
최근의 컴파일러들은 fortran의 규격을 따르고 있다는데 이게 뭘까

 Analysis part
 
 - Lexical analyzer
 - Syntzx analyzer
 - Semantic analyzer

Synthesis part

 - Intermidiage code generator
 - Code optimizer
 - Code generator

모든 과정에서 Symbol Table이 사용된다. 오토마타랑 파싱할 때 배웠던 그런거인듯

1. Lexical analyzer
	A = B + C를 'A', '=', 'B' 처럼 유의미한 최소 단위인 토큰으로 나눠줌.
	
 





 


	
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE5NTE1NjU5MTYsMjY4NTE0MTkwLC0xNj
MzMTc3MDE2LC00MDM3ODczODMsLTE0MTY3ODMwNzBdfQ==
-->