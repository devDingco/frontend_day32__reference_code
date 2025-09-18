## 과제 요구 사항
### 레퍼런스 코드에 사용된 OPEN API
고양이 이미지를 불러오는 API를 사용했어요.
 - API 키 발급이 필요하고, 회원 가입 후에 API 키를 발급받을 수 있습니다.
 - <a href="https://developers.thecatapi.com/view-account/ylX4blBYT9FaoVd6OhvR?report=bOoHBz-8t">API 사용 방법</a>
 - 환경변수:
   - `NEXT_PUBLIC_API_URL`=https://api.thecatapi.com/v1/images/search?limit=10&breed_ids=beng
   - `NEXT_PUBLIC_API_KEY`="발급 받은 API 키를 넣어주세요!"

### **공통**

- [ ]  `day31` 폴더의 코드를 기반으로 `day32` 을 완성해 주세요.

### **게시글 작성**

- [ ]  게시글 작성 컴포넌트를 **리팩토링**해 주세요.
    - **경로:** `src/components/boards-write/index.tsx`
    - **제목·내용·글쓴이** 3개의 input을 **하나의 state**로 통합합니다.
    - 각 input의 변경을 처리하던 **세 개의 함수**도 하나의 함수로 통합합니다.

### **나만의 컨텐츠 목록 – 오픈 API**

- [ ]  오픈 API를 사용해 **나만의 컨텐츠 목록** 페이지를 구현해 주세요.
    - **페이지 경로:** `src/app/openapis/page.tsx`
    - **컴포넌트 경로:** `src/components/openapis-list/index.tsx`
    - 오픈 API 종류는 자유입니다. (예: 강아지 목록, 고양이 목록 등)
    - 디자인, 무한 스크롤, 페이지네이션 등 기능에 **제한 없이 자유롭게 구현**합니다.
    - 페이지에서 직접 작성하지 말고, **컴포넌트를 만들어 조립**해 주세요.

### **컴포넌트 리팩토링**

- [ ]  나만의 컨텐츠(오픈 API) 컴포넌트를 **타입스크립트 적용 및 파일 분리**로 보완해 주세요.
    - 타입 에러가 감지되는 부분을 타입 정의로 해결합니다.
    - 유지보수를 위해 아래와 같이 파일을 분리합니다.
        - hook.ts
        - index.tsx
        - queries.ts
        - styles.module.css
        - types.ts
