# TECH-Solidity-Study
솔리디티 스터디

# Guide

## repository(레파지토리) 구조

```
TECH-Solidity-Study
   **| yourId (branch)**
       │
       ├─  solidity_docs (dir)
       │    ├─ XXX.md
       |    ├─ ...
       ...

   **| SHL3 (branch, 예시)**
       │
       ├─  solidity_docs (dir)
       │    ├─ XXX.md
       |    ├─ ...
       ├─  web3oj (dir)
       │    ├─ ...
       ├─  강의필기 (dir)
       ...
  
   ...
```

**필수 directory : solidity_docs**

이외의 dir 구조는 solidity라는 주제에 크게 벗어나지 않는 한 특별한 제약사항은 없다.

## 스터디 방식

기한 : **매주 수요일 오후 3시 이전**까지 PR을 날린다.

범위 : 따로 고지함

## 스터디 참여 방법

**["TECH-Solidity-Study" 레파지토리로부터 내 레파지토리 만들고(fork), 로컬에 복제하기(clone)]**

1. "HIBL-2G의 TECH-Solidity-Study" 레파지토리를 fork한다(이때, "Copy the main branch only”를 체크 해제).
    - 상단 fork 버튼 클릭
2. fork한 레파지토리를 로컬 컴퓨터에 clone한다.
    - git clone [내 레파지토리 주소]
3. 연결된 원격 저장소 확인 후 upstream을 추가한다.
    0. `git init` : 로컬의 작업공간 초기화하기
    1. `git remote add origin "내 레파지토리 주소"` 로 origin을 설정한다.
    2. `git remote add upstream "HIBL-2G의 TECH-Solidity-Study 레파지토리 주소"` 로 upstream을 설정한다.
    3. `git remote -v`로 upstream 추가 여부를 확인한다.
        
        ```jsx
        origin "자신의 레파지토리 주소" (fetch)
        origin "자신의 레파지토리 주소" (push)
        upstream "HIBL-2G의 레파지토리 주소" (fetch)
        upstream "HIBL-2G의 레파지토리 주소" (push)
        ```
        
    
    *origin과 upstream은 원격 레파지토리 주소 저장 변수이다.
    

모든 과정이 끝나면, 로컬의 작업 환경을 만든 것이다.

앞으로의 로컬 작업에서는 하단 내용만 참고하면 된다.

**[로컬에서 작업하고 작업물을 공유하기]**

0. `git status`로 현재 위치한 branch를 확인한다. 
    만약 자신의 branch가 아니라면,** (로컬에서 처음 생성시)`git checkout -b "자신의브랜치명"` 혹은 (브랜치 생성이 돼있다면)`git switch "자신의브랜치명"`으로 branch를 변경한다.**
2. 개별 브랜치가 없다면, 개별 브랜치를 만들어서 그 위에 작업한다. 이때 브랜치명은 자신의 깃허브 아이디로 한다.
3. **작업 전, `git pull upstream` 으로 원격 저장소와 로컬 저장소를 동기화**시켜준다.
    - 원격 레파지토리의 변화를 로컬에 반영할 수 있다.
4. 작업을 한다.
5. 변경된 파일을 staging 후 commit하고(각자 서치), **origin**의 **자신 브랜치에** push한다
    - `git push origin “자신의브랜치”`
    
    **주의사항 : upstream에 푸시하지 않는다.**
    
    origin(자신의 레파지토리)에 푸시해야하므로, upstream(”TECH-Solidity-Study ”레파지토리)에 푸시하지 않도록 한다. 이때 upstream 설정 여부는 `git remote -v`로 확인 가능하다.
    
5. 성공했다면 자신의 원격 레파지토리(깃허브)에서 push한 작업물이 보일 것이다.
6. "TECH-Solidity-Study" 레파지토리에 작업 내용을 공유하기 위해 pull request를 보낼 수 있다.
    - Create Pull Request 버튼을 클릭한다.
    - PR은 스터디장에 의해 거부될 수 있으며, 거부 시 고지할 것이다.

## commit message 작성법

각자 학습을 목적으로 하는 스터디이므로 커밋 메시지는 자유형식으로 한다.

다만 무슨 내용이 담겨있는지 알기 쉽게 하도록 하는 것을 추천한다.

또, 커밋 단위는 큰 것보다는 작은 것이 좋다.

### PR의 목적

제출 확인과 피드백.

---

### reference

- [HongikB612](https://github.com/HongikB612)/**[algorithm-study](https://github.com/HongikB612/algorithm-study)**
- [GDSC-Hongik](https://github.com/GDSC-Hongik)/**[Effective-Typescript](https://github.com/GDSC-Hongik/Effective-Typescript)**
- [GDSC-Hongik](https://github.com/GDSC-Hongik)/**[GDSC-1st-Backend-Study](https://github.com/GDSC-Hongik/GDSC-1st-Backend-Study)**
- [https://github.com/ROUTINE-STUDY/Algorithm/tree/main/Baekjoon](https://github.com/ROUTINE-STUDY/Algorithm/tree/main/Baekjoon)
