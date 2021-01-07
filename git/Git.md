# Git

> DVCS, 분산버전관리시스템



## 로컬 저장소 설정

```bash
$git init
(master) $
```

* `.git` 숨김 폴더가 생성된다.
* `(master)` 브랜치 표기



## 기본 흐름

> 어떠한 작업 => `$ touch 파일명`

```bash
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        1.txt

nothing added to commit but untracked files present (use "git add" to trach)
#커밋할 파일X(Staging Area X)
#but, untracked files 있음(Working Directory O)
```

## add

```bash
$ git add . #현재 디렉토리(하위까지)
$ git add a.txt  #특정 파일
$ git add test/  #특정 폴더
```

```bash
$ git add .
$ git status
On branch master

No commits yet
#커밋이 될 변경사항들 (SA O)

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   1.txt
```



## commit

> 스냅샷, 버전 새롭게 만든다.

```bash
$ git commit -m '커밋할 메시지'
```

* 해시값이 고유 커밋을 의미

  예)  `13ea848f7901fab549db49818931cba963664b79 `

* 커밋 메시지는 반드시 현재 작업 내용을 나타낼 수 있도록 잘 작성하는게 중요하다.

## 기타 상태 명령어

### status -> WD, SA 파일 상태 확인

### commit  -> 버전 확인



