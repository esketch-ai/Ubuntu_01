FROM python:3.10.0

ENV PYTHONUNBUFFERED 1

LABEL yh Bang <yh20studio@gmail.com>
# Docker의 컨테이너를 생성 및 관리 하는 사람의 정보를 기입해줍니다.

RUN pip install django
# python 이미지 상에 django를 pip를 통해 설치합니다.

RUN mkdir /srv/letter_web

WORKDIR /srv/letter_web
# CMD에서 설정한 실행 파일이 실행될 디렉터리를 지정해주어야 한다.

COPY ./requirements.txt ./            

RUN pip3 install -r requirements.txt  

COPY . .

CMD ["uwsgi", "--ini", "uwsgi/uwsgi.ini"]
# uwsgi로 실행할 수 있도록 cmd 교체

EXPOSE 8000
