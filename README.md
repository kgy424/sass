# sass는 거의 사용 안 함 --> scss를 사용 함. 사스라고 읽음



### 1. 비주얼 스튜디오 코드에 "Live Sass Compiler" 설치

![image](https://github.com/kgy424/sass/assets/129706828/e509ef16-5539-4920-8d3a-8768d8d5fcef)


### 2. scss 컴파일

![image](https://github.com/kgy424/sass/assets/129706828/b0f764e9-8500-4e2b-ae28-35688fba9228)


### 3.css 위치변경 

![image](https://github.com/kgy424/sass/assets/129706828/1d7e6050-8470-49d8-90be-07b00e1863d1)


### 4. savePath:null이면 scss파일과 같은 위치에 style.css가 생긴다

![image](https://github.com/kgy424/sass/assets/129706828/e218d64e-1bb2-492d-a355-53b795512a4f)


### 5.  savePath에 "~/css"치면 해당 파일 안에 css 폴더가 생김

![image](https://github.com/kgy424/sass/assets/129706828/5536a31e-c25c-4773-9f6b-56706b6767fc)

### 6. savePath에 "~/../.css"치면 상위 폴더 안에 css 폴더가 생김

![image](https://github.com/kgy424/sass/assets/129706828/2fdcb8c0-946e-46ca-96cf-54920c48396c)


# 주석처리방법

- /* 이거는 css랑 연동(컴파일)되는 주석 */
- // 이거는 연동 안 되는 주석
![image](https://github.com/kgy424/sass/assets/129706828/b759ee91-bf2c-4c54-ac2b-ec7a78fbb95b)


# 변수 만들기
## --> $로 시작함. 영문, 숫자, -, _ 만 사용 가능. 숫자로 시작 불가능
![image](https://github.com/kgy424/sass/assets/129706828/8724fe88-dd4e-4568-bd20-83282a39d209)
\

# Partials(파샬)
 - 관련된 것끼리 묶어서 분리/ 소스에 반복되는 부분들을 분리, 분산 시켜서 모듈화 시키는 기능

   * partials의 파밍명은 "_" 로 시작하며
   * 불러들일때에는 @import '파일명'  --> 이 때는 파일명에 "_"는 포함시키지 않고 확장명도 포함시키지 않는다.

  👶 Scss는 _로 시작하는 파일은 컴파일 하지 않는다.

![image](https://github.com/kgy424/sass/assets/129706828/6c3808ac-c021-4e00-aabc-3c5ca740065a)


# 💖 변수를 부르는 방법

      ✔️ @import --> 변수가 중복될 때 아래의 것이 적용된다.

![image](https://github.com/kgy424/react_basic/assets/129706828/ebc0d11a-3abe-44b2-b63a-41bcd2c56d6d)

      ✔️ @use --> 변수 이름이 같을 때 에러 발생, @use를 사용할 때는 앞에 파일명을 추가해서 파일명.변수명으로 부르면 해당 변수를 부를 수 있음.
    
![image](https://github.com/kgy424/react_basic/assets/129706828/fb584029-99cf-40d8-a5c3-6ff607694852)

    ✔️ as뒤에 별명을 붙여서 사용 할 수 있음.
    
![image](https://github.com/kgy424/react_basic/assets/129706828/035da33c-b6fe-416f-a7fd-f621295ef67f)

     ✔️ @forward는 파샬을 묶어줌. style.scss에서는 _index.scss를 호출하여 사용함.
![image](https://github.com/kgy424/react_basic/assets/129706828/d1b5ed4a-7486-44a1-ad01-e63eaa8436d5)

    ✔️ *(와일드카드) 를 붙이면 이름을 생략할 수 있음.
![image](https://github.com/kgy424/react_basic/assets/129706828/0fb9fb10-ef13-496c-b02f-b0d7779a499a)
