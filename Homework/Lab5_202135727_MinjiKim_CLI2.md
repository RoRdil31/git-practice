# CLI 2

## I/O Redirection, Expansion, Backslash

- Standard Output (default : screen)
    - **>**:다른 곳으로 output 출력 가능.
        - cat으로 해당 text file의 내용 출력.
        
        ![image.png](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/CLI2/image%2012.png?raw=true)
        
    - **>>**:기존 file 내용 뒤에 추가.
        
        ![image.png](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/CLI2/image%2013.png?raw=true)
        
- Standard Input
    - **sort < words.txt** (words.txt를 정렬한 것을)
    - **>sorted_words.txt** (에 저장)
    
    ![image.png](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/CLI2/image%2014.png?raw=true)
    
- Expansion : echo (*, ~)
    
    ![image.png](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/CLI2/image%2015.png?raw=true)
    
- Tip : Backslash
    
    ![image.png](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/CLI2/image%2016.png?raw=true)
    

---

## Permission, Superuser

Linux는 multi-user system 임 ⇒ Owner, Group, Others로 나뉨.

![image.png](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/CLI2/image%2017.png?raw=true)

- Changing Permissions
    
    ![image.png](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/CLI2/image%2018.png?raw=true)
    
    ![image.png](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/CLI2/image%2019.png?raw=true)
    
- Superuser
    
    ![image.png](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/CLI2/image%2020.png?raw=true)
    

---

## Text Editors, Shell Script, History

- Text Editors (키보드로만 문서 작업)
    
    Linux에서, CLI-based or GUI-based text editors 존재.
    
    - Command line
        - vi, vim
        - Emacs
        - nano
    - Graphical
        - gedit
        - kwrite
- Shell Script
    
    Write and run a shell script
    
    ![image.png](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/CLI2/image%2021.png?raw=true)
    
    현재 작업 중인 directory에 해당 file이 없으면 새롭게 만듦.
    
- Tip : History
    
    ![image.png](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/CLI2/image%2022.png?raw=true)
    

---

## wget, curl, grep

- wget
    
    현재 작업중인 directory로 파일 다운.
    
    ![image.png](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/CLI2/image%2023.png?raw=true)
    
- curl
    
    fetching, uploading, and managing data over the Internet
    
    ![image.png](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/CLI2/image%2024.png?raw=true)
    
- grep
    
    ![image.png](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/CLI2/image%2025.png?raw=true)
    
