# 세팅

<img src="https://github.com/limtowoong/blog/assets/104752202/b84f9a06-6544-4e3f-96af-344b5934347f" width="600" height="600"/>

Spring Initializr에서 압축 파일을 다운 받아준다.

<br>

<img src="https://github.com/limtowoong/blog/assets/104752202/ec93d0bd-9eea-4285-9e29-ad6281bc9cc3" width="600" height="600"/>

다운 받은 압축 파일을 원하는 위치에 푼다.

<br>

import -> Gradle -> Existing Gradle Project

개발 툴을 실행하여 파일을 import 해줍니다.

<br>

# 빌드 과정

<img src="https://github.com/limtowoong/blog/assets/104752202/a7fd91ed-6990-461c-a9e6-c781bbecab74" width="600" height="400"/>

위에서 설치한 파일에 경로를 복사한다.

<br>

<img src="https://github.com/limtowoong/blog/assets/104752202/a30cec3b-18c4-4719-9dfa-3a626ac4d533" width="400" height="300"/>

터미널 실행

<br>

<img src="https://github.com/limtowoong/blog/assets/104752202/bc266f87-89bc-4700-9cc8-0e4abed4ea77" width="600" height="300"/>

`cd C:\Users\Office\Downloads\demo(복사한 파일 경로)` 를 입력하면 해당 파일 경로로 이동한다.

<br>

만약 실수로 파일 경로를 잘못 입력 했다면 `cd..`를 쓰면 된다.

<br>

<img src="https://github.com/limtowoong/blog/assets/104752202/d296ad7b-58df-455e-ad69-4fb60096ad2c" width="600" height="500"/>

ls를 입력해서 하위 폴더 목록들을 보면 `gradlew`라는 폴더가 있는데, 이 폴더에 build 폴더를 생성할 것이다.

<br>

<img src="https://github.com/limtowoong/blog/assets/104752202/25116b05-3966-4295-b8c1-d0d4db63b799" width="600" height="200"/>

`.\gradlew build`를 입력해서 BUILD SUCCESSFUL이 나오면 성공한 것이다.

<br>

<img src="https://github.com/limtowoong/blog/assets/104752202/97e39f82-d649-4838-a217-6381425c191b" width="600" height="300"/>

다시 ls를 입력하면 build 폴더가 생성된 것을 볼 수 있다.

<br>

<img src="https://github.com/limtowoong/blog/assets/104752202/522827d3-6c80-4cca-b534-a5fdc507c207" width="600" height="300"/>

cd로 build 폴더에 이동하고 ls로 폴더 목록을 확인해 보면 libs 폴더가 있다.

<br>

<img src="https://github.com/limtowoong/blog/assets/104752202/81171a8b-c9b9-4463-a5f4-d8e23f3ebe59" width="600" height="200"/>

cd로 libs 폴더에 이동하고 ls를 사용하면 jar 파일을 확인할 수 있다.

<br>

![image](https://github.com/limtowoong/blog/assets/104752202/78c2b913-5e82-4c30-8012-37a563b811b2)

`java -jar .\demo-0.0.1-SNAPSHOT.jar(jar 파일 이름)`를 입력하면 빌드가 되는 것을 볼 수 있다.

이제 웹 서버가 켜진 것을 볼 수 있다.

# 빌드 취소하는 법

ctl + c 를 누르면 입력창이 뜬다.

`cd..`를 사용해서 `C:\Users\Office\Downloads\demo` 이 경로까지 온다.

그 후 `gradle clean`와 `gradle build clean`을 순서대로 입력하면 웹 서버가 꺼진다.
