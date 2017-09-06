# Docker 이미지 생성시 베이스가 될 이미지 정보
FROM node:6.11.2

# Dockerfile 생성/관리자
MAINTAINER JungMin Ahn <dkswjdals89@bbros.kr>

# App 디렉토리 생성 및 워크 디렉토리 지정
RUN mkdir -p /user/src/app
WORKDIR /user/src/app

# 소스 코드 파일을 워크 디렉토리로 복사
ADD ./app /user/src/app

# npm package install
RUN npm install

# Port 지정
EXPOSE 3000 80


# 컨테이너에서 실행할 명령 지정
CMD [ "npm", "start" ]