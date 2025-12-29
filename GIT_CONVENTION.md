# Git Commit Message Convention

본 문서는 회사 내 모든 Git 저장소에서 사용하는 **Commit Message 작성 규칙**을 정의한다.  
모든 커밋은 아래 규칙을 기준으로 작성하는 것을 원칙으로 한다.

---

## 1. Commit Message Structure

커밋 메시지는 다음 3가지 영역으로 구성된다.

```
<Title>

<Body>

<Footer>
```

- 각 영역은 **빈 줄로 구분**한다.
- Title은 필수, Body와 Footer는 선택 사항이다.

---

## 2. Title Rules

### 2.1 기본 규칙

- 제목은 **최대 50자 이내**로 작성한다.
- 첫 글자는 **대문자**로 시작한다.
- **마침표(.)를 사용하지 않는다.**
- 제목은 **명령문(Statement)** 형태로 작성한다.

#### 예시
```
Feat: Add key mapping for shortcut actions
Fix: Resolve null pointer exception on login
```

---

### 2.2 Type Prefix

모든 제목은 아래 형식으로 시작한다.

```
<Type>: <Title>
```

#### 사용 가능한 Type 목록

| Type | 설명 |
|---|---|
| feat | 새로운 기능 추가 |
| fix | 버그 수정 |
| refactor | 리팩토링 (기능 변경 없음) |
| design | CSS 등 UI/UX 디자인 변경 |
| comment | 주석 추가 또는 수정 |
| style | 코드 스타일 변경 (포맷, 세미콜론 등, 로직 변경 없음) |
| docs | 문서 추가/수정/삭제 (README 포함) |
| test | 테스트 코드 추가/수정/삭제 (로직 변경 없음) |
| chore | 기타 변경사항 (빌드 스크립트, 설정, 패키지 관리 등) |
| init | 프로젝트 초기 생성 |
| rename | 파일 또는 폴더 이름 변경만 수행한 경우 |
| remove | 파일 삭제만 수행한 경우 |

---

## 3. Body Rules

Body는 **“무엇을(What)” 그리고 “왜(Why)” 변경했는지**를 설명한다.

- 구현 방식(How)에 대한 상세 설명은 지양한다.
- 여러 줄로 작성할 경우, 각 항목은 `-` 로 구분한다.

#### 예시
```
- Prevent duplicated key registration
- Improve readability of key mapping logic
```

---

## 4. Footer Rules (Optional)

Footer는 이슈 트래킹 시스템과의 연계를 위해 사용한다.  
필수는 아니며, 필요한 경우에만 작성한다.

### 사용 가능한 키워드

| Keyword | 설명 |
|---|---|
| Fixes | 이슈를 해결 중이거나, 병합 시 자동 종료 목적 |
| Resolves | 이슈가 완전히 해결되었을 때 사용 |
| Ref | 참고용 이슈 연결 |
| Related to | 관련된 이슈가 있으나 해결되지 않은 경우 |

#### 예시
```
Fixes: #47
Related to: #32, #21
```

---

## 5. Commit Message Examples

### Example 1
```
Feat: Add Redis health check endpoint

- Provide health endpoint for Redis connectivity
- Improve observability in production environment

Related to: #99
Resolves: #101
```

### Example 2
```
Fix: Prevent duplicate user registration

- Validate email uniqueness before persistence
- Avoid unexpected constraint violation errors

Ref: #80
Fixes: #88
```

### Example 3
```
Docs: Update backend service README

- Add installation instructions
- Clarify environment variable configuration
```
