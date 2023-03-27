# 2023_OSS
## 2023 OSS 수업
<hr/>

### 3주차 git

### 이미지
![Alt text](../image/kau_test.png)

### 링크
[LMS](https://lms.kau.ac.kr)

#### ProGit 링크
[ProGit](https://git-scm.com/book/en/v2)

##### 주요 git 명령어
* add : 파일을 추적 대상으로 포함시킬 때, 또는 커밋 대상으로 포함시킬 때 사용
* commit
	* 예) git add
* git reset HEAD : stage된 파일을 unstaged로 변경
* git checkout -- : stage되어 있는 파일을 수정한 후 수정 전으로 되돌림
* branch
* merge
* status
* log
	* 예) git log --oneline --decorate --graph --all
<hr/>

### 2주차 숙제
```sh
#!/bin/bash

FILE_COUNT=$(find /home/kau2 -type f -name "w2_homework.txt" 2>/dev/null | wc -l)
if [ $(expr $FILE_COUNT) -eq $(expr 1) ]; then

	FILE_PATH=$(find /home/kau2 -type f -name "w2_homework.txt" 2>/dev/null)
	LINE_NUMBER=$(wc -l $FILE_PATH | cut -d ' ' -f 1)
	LAST_LINE=$(tail -n 1 $FILE_PATH)

	echo -e "----------"
	echo -e "name :\n"

	echo -e "\n----------"
	echo -e "student id :"

	echo -e "----------\n"
	echo -e "file path :\n$FILE_PATH"

	echo -e "\n----------"
	echo -e "line number :\n$LINE_NUMBER"

	echo -e "\n----------"
	echo -e "last line :\n$LAST_LINE"
fi
```

## 마크다운
### 목록
#### 번호 있는 목록 : 내림차순 정렬
1. 첫번째
3. 세번째
2. 두번째

#### 번호 없는 목록 : * , - , +
* 첫번째  
 
* 세번째   

* 두번째   

<hr/>

* 빨강
	* 녹색
		* 파랑

### 강조
*single asterisks*   
_single underscores_   
**double asterisks**   
__double underscores__   
~~cancelline~~   
