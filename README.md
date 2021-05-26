# DjangoTutorial

**자신의 컴퓨터 운영체제에 맞는 git을 자신의 컴퓨터에 설치해주세요**

## Step #1 - git 설치

현재 레포지토리를 자신의 레포지토리로 `fork`합니다.
![fork](https://user-images.githubusercontent.com/32446834/119656836-1ef13d00-be66-11eb-9273-2d14d3d59bcd.png)

## Step #2 - 원격 저장소 등록하기

1. 자신의 로컬 디렉토리(django tutorial directory)에서 다음 명령을 실행해주세요.

```
$ git init
```

2. 현재 위치한 로컬 디렉토리의 origin 원격 저장소(fork한 자신의 원격 저장소)를 등록합니다.

```
$ git remote add origin <fork한 자신의 원격저장소 clone url>
```

3. 그리고 Pull Request를 보내기 위해 upstream 원격 저장소(현재 BackendStudyOrg에 위치한 DjangoTutorial 저장소)를 등록합니다.

```
$ git remote add upstream <BackendStudyOrg/DjangoTutorial의 clone url>
```

4. `git pull`을 사용해 origin 원격 저장소에 있는 ReadMe.md를 로컬 저장소로 받아옵니다.

```
$ git pull origin
```

## Step #3 - 코드 수정 후 수정사항 원격 저장소로 push 하기

1. `git add`를 사용해 현재 수정한 파일들을 stage에 올립니다. (IDE를 사용해도 괜찮습니다.)

```
$ git add . # 현재 수정된 파일 전부를 stage에 올리는 명령어입니다.
```

2. `git commit`을 사용해 stage에 올라간 changes를 커밋합니다.

```
$ git commit
```

2-1. 이 때, 자동으로 vim 편집기가 열릴텐데 `i` 키를 누르고 커밋 메시지를 입력합니다.

2-2. 그리고 `esc` 키를 눌러 편집 모드에서 빠져나옵니다.

2-3. 그 상태 그대로 `:wq`를 입력하고 `enter` 키를 눌러 커밋을 완료합니다.

3. `git push origin`을 사용해 자신의 원격 저장소로 수정사항들을 push합니다.

## Step #4 - 원격 저장소에서 PR 생성해서 날리기

1. 자신의 원격 저장소에서 PullRequest 탭을 클릭합니다.

![PR탭 클릭](https://user-images.githubusercontent.com/32446834/119659182-e4d56a80-be68-11eb-960e-588545a8e672.png)

2. New Pull Request 버튼을 클릭합니다.

3. 그리고 BaseRepository에서 자신의 닉네임으로 된 브랜치를 선택한 후에 PR을 생성합니다.

![image](https://user-images.githubusercontent.com/32446834/119659550-37168b80-be69-11eb-9111-335c4c988682.png)

