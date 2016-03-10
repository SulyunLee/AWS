# Installing Wordpress on AWS
### SSH을 사용하여 인스턴스에 연결하기
1. 생성한 .pem 키의 위치가 있는 곳으로 이동

2. private key 파일을 공개적으로 볼 수 없는지 확인
`chmod 400 my-key-pair.pem`

3. ssh 명령을 사용해 instance에 연결
- Amazon Linux의 경우 user name은 ec2-user
- Ubuntu의 경우 user name은 ubuntu

`ssh -i my-key-pair.pem user-name@DNS-name`

### Apache 웹 서버 시작하기
`sudo service httpd start`

### MySQL 서버 시작
`sudo service mysqld start`
### MySQL 서버를 중단
`sudo service mysqld stop`

### Wordpress 수정
'http://ec2-52-79-131-216.ap-northeast-2.compute.amazonaws.com/wp-admin/'로 이동한다.
