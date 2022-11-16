# FTP, SFTP
- File Transfer Protocol의 약자로 파일을 전송할 때 사용하는 프로토콜이다. SFTP는 기존의 FTP의 보안 취약점을 개선한 파일 전송 방식으로 데이터를 암호화해서 전송하기 때문에 안전하게 파일을 전송할 수 있다. 최근에는 FTP를 거의 사용하지 않는다.

# Sublime Text와 FTP
- Sublime Text를 이용해서 로컬 컴퓨터에서 개발을 하고, 파일은 개발서버로 전송해야 한다면 파일을 일일이 클라이언트를 이용해서 전송하는 것은 매우 귀찮은 일이다. 안타깝게도 Sublime은 FTP 기능을 제공하지 않는다. 하지만 확장 기능이 있다. 

# Sublime SFTP 
- Sublime SFTP는 서브라임 텍스트를 이용해서 FTP, SFTP를 사용할 수 있도록 확장해주는 확장 기능이다. FTP, SFTP를 지원하고, Password 방식 뿐 아니라 SSH Key도 지원한다. 유료지만, 사용에는 제한이 없다. 가끔씩 사용권유 메시지가 뜬다. 

# 사용방법
- 해당 폴더에서 오른쪽 마우스 > SFTP/FTP > map to remote
```
host : 도메인
user : 아이디
password : 비밀번호
remote_path : 파일을 업로드 할 경로
upload_on_save : 수정사항을 자동으로 업로드
```

# 홈페이지
- http://wbond.net/sublime_packages/sftp
```
usage : 사용방법
settings : 설치방법
```
- SSH Key를 이용해서 접속하는 경우 윈도우 사용자는 SSH Key를 그대로 사용하면 안되고, PuTTYgen을 이용해서 ppk 파일로 컨버팅해서 사용해야 한다.
- 설치 https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html

- 참고 https://opentutorials.org/module/432/3738

# 추가기능
1. diff remote file : 해당 파일이 로컬과 서버에서 어느부분이 수정되었는지(다른지) 알려줌
2. sync local(로컬) -> remote(서버) : 로컬을 기준으로 서버의 내용을 바꾼다
2. sync remote -> local : 반대
2. sync both diretion : 둘다 같게 만든다
3. browse remote : 파일들의 리스트를 보여주고 원격 작업이 가능 
3. up a folder : 현재 디렉토리의 부모 디렉토리로 이동
3. folder actions : 현재 디렉토리에서의 어떠한 명령을 실행시킬 수 있음
