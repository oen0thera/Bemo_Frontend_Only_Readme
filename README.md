# 배움의 모든것 :book: : 학원 견적 매칭 서비스
<div align="center">
  <img alt="main_image" src="https://github.com/user-attachments/assets/1b32c4ba-f7fe-46db-97ae-e77c014666d6"/>
</div>

<br>

- 배포 URL : https://front.bemo.pe.kr

<br>

# 프로젝트 소개
- 배움의 모든 것(이하 배모)은 수강자 - 학원 견적 매칭 서비스입니다.
- 서비스 사용자들은 자신의 주변에 있는 학원을 카테고리/위치/나이 기반으로 검색 혹은 이름 기반으로 검색할 수 있습니다.
- 자신이 관심있는 학원에 대한 상세정보(카테고리, 소개글, 수강료, 위치, 강사소개, 시설 사진, 리뷰)를 확인할 수 있습니다.
- 견적요청을 보낸 수강희망자에게 학원이 견적서를 보내줄 수 있으며, 이에 수강자가 견적서에 제공된 정보를 통해 해당 학원과 매칭됩니다.
- 자신이 수강하고자 하는 취미를 AI 기반 취미 추천 서비스를 통해 추천받을 수 있습니다.


## 팀원 구성 및 역할

| **이름** |                                                                   **GitHub**                                                                   |                                                                                           **구현 기능 및 역할**                                                                                           |
| :------: | :--------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|  김원진  |   [<img src="https://avatars.githubusercontent.com/u/76833065?v=4" height="100" width="100"> <br/> @oen0thera](https://github.com/oen0thera)   | <ul><li>프로젝트 매니저</li><li>CI/CD 총괄</li><li>메인 페이지 및 GNB 구현</li><li>로그인/회원가입 기능 및 페이지 구현</li><li>아이디 찾기/비밀번호 찾기·변경 페이지 구현</li><li>임시저장 및 불러오기 기능</li><li>학원 상세 페이지 탭 전환 위치 조정 및 슬라이드 적용</li></ul> |
|  김나연  | [<img src="https://avatars.githubusercontent.com/u/126762806?s=64&v=4" height="100" width="100"> <br/> @Nangniya](https://github.com/Nangniya) |                       <ul><li>디자인 시스템</li><li>학원 검색 페이지 구현</li><li>카테고리/지역/나이 선택 모달 구현</li><li>통계청 지역 api 연결</li><li>favicon 및 404 페이지 구현</li>                        |
|  권시경  | [<img src="https://avatars.githubusercontent.com/u/104986866?v=4" height="100" width="100"> <br/> @kweonsikyung](https://github.com/kweonsikyung) |                                                                       <ul><li>디렉토리 구조 개편</li><li>학원 상세 페이지</li><li>로그인/회원가입 페이지 구현</li><li>카카오맵 api 연결</li><li>학원 상세페이지 탭 전환 및 스크롤 구현</li><li>토스트 기능 구현</li></ul>      | 
|  정우성  | [<img src="https://avatars.githubusercontent.com/u/101249011?s=64&v=4" height="100" width="100"> <br/> @dntjd129](https://github.com/dntjd129) |                                                                       <ul><li>마이페이지 구현</li><li>마이페이지 내 세부기능<br>(최근,찜,리뷰,견적) 구현</li><li>견적 관리 모달 및 기능 구현</li><li>AI 기반 취미 추천 페이지 구현</li></ul>       | 

<br>

## 개발 환경 및 기술 스택

- 언어 : TypeScript, Java
- 프레임워크 : Next.js (app 라우터), Spring Boot
- css: scss-module
- 클라이언트 전역상태관리: zustand
- 서버 상태관리 및 데이터 페칭 : tanstack-react-query
- DB : MySQL
- 버전 및 이슈 관리 : Github, Github Issues
- 협업툴 : Discord
- 프론트 서비스 배포환경 : Github Actions + AWS S3
- 기타 : Figma
  
<br>

## 협업 컨벤션
### 커밋 컨벤션
| Type        | Description                                 |
| ----------- | ------------------------------------------- |
| `feat`      | 새로운 기능 추가                            |
| `fix`       | 버그 수정                                   |
| `docs`      | 문서 관련                                   |
| `style`     | 스타일 변경 (포매팅 수정, 들여쓰기 추가 등) |
| `refactor`  | 코드 리팩토링                               |
| `test`      | 테스트 관련 코드                            |
| `build`     | 빌드 관련 파일 수정                         |
| `perf`      | 성능 개선                                   |
| `ci`        | CI 설정 파일 수정                           |
| `conf`      | 설정 관련 수정                              |
| `type`      | 타입과 관련된 작업                          |
| `asset`     | 애셋 파일 추가                              |
| 'rename'    | 파일 및 디렉토리 이름 변경                   |
| 'chore'     | 기타 변경사항                              |

<br>

### 이슈 컨벤션
1. 제목은 `Subject : 제목` 형식으로 작성하며 커밋 컨벤션과 동일하게 subject를 작성한다.

   > 💡 Issue의 subject는 파스칼 케이스로 작성한다.

2. 구현할 기능 혹은 질문할 내용에 대해 상세히 기술한다.

3. 이슈에 맞는 Label을 지정하고 생성한다.
   > 💡 만일 상황에 맞는 Label이 존재하지 않는 경우 새로운 Label을 생성한다. 이 경우 상호 보고 이후 생성한다.
   > 💡 본인 이름의 Label 생성 후 연결하여 상호 같은 이슈에 대한 중복 작업을 방지한다.
   > 💡 이슈를 해결했을 경우 PR에 해당 이슈를 연결 후 이슈를 종료한다.

<br>

### eslint, prettier
- 정해진 규칙에 따라 코드 스타일을 정리해 코드의 일관성을 유지하고자 한다.
- 코드 품질 관리는 eslint에, 코드 포맷팅은 prettier로 사용.

<br>


