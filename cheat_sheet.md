# 1. Command 명령어(터미널 명령어)

#### 관리자 권한	
* 관리자 권한으로 실행	``` $ sudo 명령어 ```

#### 디렉토리 위치 이동	
* 홈 디렉토리로 이동	``` $ cd ~ ```
* 디렉토리로 이동	```$ cd 디렉토리이름```
* 상위(부모) 디렉토리로 이동	``` $ cd .. ```

#### 디렉토리 정보 출력	
* 현재 위치 출력	```$ pwd```
* 디렉토리 안의 파일 출력	```$ ls```
* 상세정보까지 출력	`$ ls -l`
* 숨김파일까지 출력	`$ ls -a`
* 숨김파일/상세정보까지 출력 `$ ls -al`
#### 생성 및 옮기기/삭제	 
* 디렉토리 생성	`$ mkdir 디렉토리이름`
* 파일 생성	`$ touch 파일이름`
* 파일 생성 및 수정	`$ echo 파일내용 > 파일이름`
* 파일이나 디렉토리 옮기기	`$ mv 옮길파일 옮겨질위치`
* 파일 이름 변경	`$ mv 바꿀파일 바꿀이름`
* 파일이나 디렉토리 복사	`$ cp 복사할파일/폴더이름 복사할경로or이름`
* 파일 삭제	`$ rm 파일이름`
* 디렉토리 삭제	`$ rm -r 디렉토리이름`
#### 기타 자주쓰는 명령어 
* 파일 내용 확인하기	`$ cat 파일이름`
* 터미널 정리하기	`$ clear`
* 이전 명령어 확인	`$ history`
* 종료	`$ exit`

# 2. git 명령어

#### 시작 및 설정	
* 설치된 git 버전 확인	`$ git --version`
* .git 하위 디렉토리 생성	`$ git init`
* 사용자 이름 설정	`$ git config --global user.name "사용자이름"`
* 사용자 이메일 설정	`$ git config --global user.email "사용자이메일"`
* 상태 확인	`$ git status`
#### 저장소	        
* 원격 저장소 연결	`$ git remote add origin [github 저장소 주소]`
* 저장소 확인	`$ git remote -v`
* 로컬 저장소 복제	`$ git clone /로컬/저장소/경로`
* 원격 저장소 복제	`$ git clone 이름@호스트:/원격/저장소/경로`
#### commit 명령어	
* 커밋에 변경사항 올림	`$ git add 파일명`
* 수정한 전체파일 올림	`$ git add .`
* 커밋 생성(변경사항 저장)	`$ git commit -m "메세지"`
* 커밋 내역 확인	`$ git log`
* 파일 상태 확인	`$ git status`
#### branch 명령어	
* 브랜치 목록 확인	`$ git branch`
* 브랜치 생성	`$ git branch 브랜치명`
* 브랜치로 이동	`$ git checkout 브랜치명`
* 브랜치만들고 이동	`$ git checkout -b 브랜치명`
* master 브랜치로 돌아옴	`$ git checkout master`
* 브랜치 삭제	`$ git branch -d 브랜치명`
* 한 커밋씩 출력	`$ git log --oneline`
* 커밋을 그래프로 표시	`$ git log --branches --graph`
#### push 명령어	    
* 원격 저장소에 업로드	`$ git push origin master`
* 커밋을 원격 저장소에 업로드	`$ git push 저장소주소 브랜치이름`
* 커밋을 원격 저장소에 업로드	`$ git push -u 저장소주소 브랜치이름`
* 클라우드 주소 등록	`$ git remote add origin 저장소주소`
* 클라우드 주소 삭제	`$ git remote remove 저장소주소`
#### merge 명령어	
* 원격 저장소 변경사항 가져오고 병합하기	`$ git pull`
* 현재 브랜치에 다른 브랜치 병합	`$ git merge 다른브랜치이름`
* 파일 병합	`$ git add 파일이름`
* 병합 이전의 내용과 비교	`$ git diff 브랜치이름 다른브랜치이름`
#### 로컬 명령어	    
* 변경 전으로 되돌림	`$ git checkout --파일명`
* 현재 상태를 다운로드	`$ git fetch origin`