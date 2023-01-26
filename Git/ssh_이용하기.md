## ssh

id_rsa : private key

id_rsa.pub : public key

id_rsa 파일을 생성할 때 id_rsa.pub파일이 저장되어있는 컴퓨터에 접속할 때 비밀번호 따로 입력하지 않아도 됨, 자동로그인 해줌 

private key는 절대 노출되어서는 안됨

id_rsa와 id_rsa.pub의 짝을 이루는 비밀번호를 통해서 자동으로 로그인하고 업로드해줌



## 방법

```
ssh-keygen
```

: 경로확인

```
cd ~/.ssh
```

:.ssh로 경로 이동

```
cat id_rsa.pub
```

:id_rsa.pub의 내용 출력 후 복사→**깃헙으로 이동**→setting→SSH and GPG keys→New SSH key→붙여넣기 후 등록 → ssh 주소 복사 → git bash 'git clone 주소 리퍼지토리 명'



