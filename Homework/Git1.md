# Changes vs Snapshots
![](images/Git1/image.png)
-> Git은 snapshots 방식.
# Local, Centralized, and Distributed Version Control
![](images/Git1/image(1).png) <br>
-> **Centralized** : 중앙 server에 매우 의존.(중앙 서버 down시 사용 X)<br>
-> **Distributed** : Centralized 단점 보완 → 각각의 local computer에서도 Version DB를 가지고 있음. local computers 간에 직접적인 communication 가능.<br>
# Three States in Git
![](images/Git1/image(2).png)<br>
→ 수정한 것을 Staging Area에 올리고 나서 commit을 해야 새로운 version이 만들어 짐.
# Git config : first-time setup
1. System level : 컴퓨터 사용하는 모든 사용자에게 적용.
    
    file : `/etc/gitconfig`
    
2. Global (user) level : current user의 모든 repositories에 영향.
    
    file : `~/.config/git/config`
    
3. Local level : current repository에만 적용.
    
    file : `.git/gitconfig`
    

`$ git config --global user.name “Minji Kim”`

`$ git config --global user.email rlaalswl1151@naver.com`

`$ git config --global init.defaultBranch main` ← master에서 바꾸는 게 아니라면 할 필요 없음.

`$ git config --list`

`$ git config --list --show-origin` ← 설정된 config level 확인 가능.

`$ git config user.name` ← 위에서 입력한 이름C 출력

# init, status, add, rm(Unstage), ignore, commit, change
- init `$ git init`<br>
- status `$ git status`<br>
  ![](images/Git1/image(3).png)<br>
  → Untracked files : git이 tracking 하지 않는다 == git과 상관 X.<br>
- add<br>
  특정 file을 staging area로 올림.<br>

  `$ git add README.md` ← git add . 하면 모든 파일 올라감.

  `$ git status`

  ![](images/Git1/image(4).png)<br>
  → commit할 준비가 되어있다는 뜻.<br>
  ![](images/Git1/image_nano.png)<br>
  ->  파일 하나를 수정하면 changes not staged for commit 에 해당 파일이 적힘.<br>

- Unstaging<br>
  ![](images/Git1/image(5).png)<br>
- Ignoring<br>
  ![](images/Git1/image(6).png)<br>
  → .gitignore라는 히든 파일이 생성된 것이고 이 파일 안에 적힌 파일 이름들을 전부 무시하게 됨.<br>
  - .gitignore file<br>
       - `*.a` ← .a 파일을 전부 무시.
      - `!lib.a`
      - `/TODO`
      - `build/` ← build 안에 있는 모든 파일 무시.
      - `doc/*.txt` ← doc 안에 있는 모든 txt 파일 무시.
      - `doc/**/*.pdf` ← doc 안에 있는 모든 하위 폴더의 pdf 파일 무시.
- Commit<br>
  ![](images/Git1/image(7).png)<br>
  git log → 그동안 commit했던 history 확인 가능.<br>
- Change branch name<br>
  ![](images/Git1/image(8).png)<br>

