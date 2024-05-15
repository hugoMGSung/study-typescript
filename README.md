# study-typescript
타입스크립트 학습 리포지토리

## TypeScript 개요
- Javascript에 **정적타입**이 추가된 프로그래밍 언어

### 역사
- 1995년 Javascript가 발표된 후 사용처가 기하급수적으로 증가
- **동적 타입 언어**(실행시 변수의 타입을 언어가 지정하는 언어) 이다 보니 버그가 많이 발생
- 반대는 C, C#, Java와 같은 **정적 타입 언어**
- 컴파일 시점에 타입 체크를 진행하고 통화하지 못하면 실행을 금지
- TypeScript = Javascript + Type 

## 개발환경

### 개발환경 설정
- Node.js 설치 [홈페이지](https://nodejs.org/en)
	- 설치 오류 error 2503, 2502
	- 콘솔 관리자모드로 실행 후 
	- msiexec/package node-v20.xx.x-x64.msi 실행

	```shell
	> node --version
	v20.12.2

	> npm --version
	10.5.0
	```

- TypeScript 설치
	- npm으로 설치

	```shell
	> npm install -g typescript
	```

### TypeScript 실행 테스트
- 타입스크립트 파일 생성
	- *.ts로 생성
	- Javascript로 코딩
	- 터미널에서 컴파일

	```shell
	> tsc file.ts
	```

	- js로 변경된 파일 node로 실행

	```shell
	> node file.js
	```

	- 자동컴파일 설정하기
		- tsc -w **파일경로** 로 해당경로에 파일이 저장할때 마다 자동 컴파일
		- tsc -w **ts파일** 

### 오류 해결방법
#### about_Execution_Policies
- 권한
	```shell
	> Get-ExecutionPolicy RemoteSigned
	```

## Type
### 타입스크립트 기본 타입
- 리스트
	1. number
	2. string
	3. boolean
	4. void
	5. null
	6. undefinded
	7. object
	8. array
	9. tuple
	10. enum
	11. any
	12. unknown
	13. never

### 변수 타입선언
- 기본 타입
	```javascript
	let name: string;
	let age: number;
	```

### 타입추론
- 컴파일러가 타입 추론. 이전의 자바스크립트와 차이가 없음

### never 타입
- 절대 반환을 하지 않는 함수

