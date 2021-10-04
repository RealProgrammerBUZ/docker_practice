FROM python:3.8

RUN apt-get update

# 컨테이너 내 주소
WORKDIR /usr/src/app

# reqirements.txt 복사 후 설치
COPY requirements.txt ./
RUN pip install -r requirements.txt

# 장고 코드 복사하사
COPY . .

# docker 컨테이너 8000포트 열어주기
EXPOSE 8000
# 쟝고 가동시켜주는 명령어
CMD [ "python", "manage.py", "runsurver", "0.0.0.0:8000" ]

