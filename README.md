# 1. Github Template Project (ver 1.0)

## Project Overview

해당 프로젝트는 GithubActions CICD Script를 프레임워크 별로 템플릿을 제공합니다. 
또한 ISSUE, PR, README Convention을 수립하여 가이드 및 템플릿으로 제공하고 있습니다. 

---

## Skills

Deploy: GithubActions

---

## Person in charge

Oner: paul.seo

E-mail: paul.seo@systrankorea.com

---

# 2. How to use

1. `.github/workflows/*`에 Spring, FastAPI, React Deploy CI Template Script가 존재합니다. 각 스크립트에서 필요로 하는 `inputs`를 확인하고 호출 스크립트를 작성해서 `ex) SYSTRAN-KOREA-AI/.github/.github/workflows/deploy-spring-template.yml@main` 다음과 같이 Checkout을 통해 사용하면 됩니다.
2. `.github/ISSUE_TEMPLATE/*`에는 feature, refactor, bug, test 관련 이슈 템플릿이 존재합니다. 타겟이 되는 프로젝트 Root 경로에 `.github/ISSUE_TEMPLATE/`를 똑같이 만들고, 템플릿을 COPY & PASTE를 진행합니다.
3. `.github/pull_request_template.md`도 같은 경로에 타겟이 되는 프로젝트 Root 경로에 `.github`를 똑같이 만들고, 템플릿을 COPY & PASTE를 진행합니다.
4. Root 경로에 위치한 `README_EXMAPLE.md`을 참고해서 `README_TEMPLATE.md` 기반으로 `README.md` 작성을 합니다.  
5. Root 경로에 위치한 `GIT_CONVENTION.md`을 참고해서 `Git Commit`을 작성합니다.

---