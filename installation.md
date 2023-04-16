가상환경 실행
venv/Scripts/activate 실행해야함
source 경로/activate
source activate
가상환경 나가기
deactivate 

ERROR: Can not perform a '--user' install. User site-packages are not visible in this virtualenv.
가상환경에서 pip 설치가 안됨 --user옵션은 가상환경에서 설치를 할 경우에 발생하는데 자동으로 --user가 되도록 설정되어있다

### resolve 1
-> https://bobbyhadz.com/blog/python-error-can-not-perform-user-install
1.Open your venv folder.
2.Click on the pyvenv.cfg file.
3.Set the include-system-site-packages property to true.
    -> Scripts/pyvenv.cfg 에 존재
4.Save the file.
5.Rerun the pip install command.
: 전역으로 바꾸는 방법이라서 의미 없음

### resolve 2 
--user 옵션을 꺼야 하는데 pip.ini 파일 내에서 
[global]
user=false
의 설정을 해야 한다고 한다
----진행중----
