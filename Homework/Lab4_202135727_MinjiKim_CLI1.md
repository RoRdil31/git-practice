![](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/shell_kernel.jpg?raw=true)
# Arguments
**[directory name]** <br>
/ root<br>
. current directory<br>
.. upper-level directory<br>
~ home of current user<br>
/[directory name] : absolute path<br>
./[directory name] : relative path<br>
../[directory name] : relative path<br><br>

# 기본적인 명령어
```sh
pwd : current path in a hierarchical directory
cd : change directory
ls : list files and directories
	-l : detailed information 보여줌 (long format)
	(-l /etc /bin : /bin과 /etc directory 안에 내용을 long format으로 보여줌)
	-lh : (위와 같음) but, 파일 size를 직관적으로 볼 수 있음.
	/bin : /bin directory의 내부 파일 보여줌.
	-la .. : 모든 파일 보여줌 (.으로 시작하는 hidden files까지 보여줌)
	
clear : kernel 창 클리어.

```
<br>

# Manipulation (조심해야 하는 명령어)
## 1. 복사 : cp
```sh
cp -r ../folder1 ./new_folder : 폴더 복사 (여러개는 -r 안씀)
	file1 file2 (이때 file2가 존재하면 file1 내용으로 overwrite)
	file1 dir1 (file1을 dir1디렉토리 안으로 복사. 이때 파일 이름 동일)
	-R dir1 dir2 (디렉토리 자체를 복사)
```
![](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/cp.png?raw=true)
## 2. 잘라내기 : mv
```sh
mv README.md LICENSE.md (이름 바꾸기)
	LICENSE.md ../ (상위 폴더로 이동)
	
	file1 file2 dir1 (file1,2가 dir1로 이동) (dir1이 없으면 error)
	dir1 dir2 (dir2가 존재하지 않으면, dir1 이름이 dir2로 rename.)
						(dir2가 존재하면, dir1이 dir2로 움직임.)

```
![](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/mv.png?raw=true)
## 3. 영구 삭제 : rm
```sh
rm LICENSE.md
	file1 file2 fi.. (여러개 가능)
	-r dir1 dir2 (directories를 지울 땐 반드시 -r 해줘야 함)

```
![](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/rm.png?raw=true)
## 4. Directory 생성 : mkdir
```sh
mkdir asset
```
![](https://github.com/RoRdil31/Open-Source-SW/blob/main/images/mkdir.png?raw=true)
## 5. Wildcards
```sh
* (모든 파일)
g* (g로 시작하는 모든 파일)
b*.txt (b로 시작하고 .txt로 끝나는 모든 파일)
Data??? (Data 다음 3개의 characters가 오는 파일)

cp *.txt text_files
mv dir1 ../*.bak dir2 (dir1, 상위 directory에서 .bak로 끝나는 모든 파일을 dir2로 이동)
rm *~ (~로 끝나는 모든 파일 삭제)
```

## 6. Help,man command
```sh
help cd

man cp

exit (터미널 종료)
```
