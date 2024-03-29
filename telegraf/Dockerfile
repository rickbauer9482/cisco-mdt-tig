FROM telegraf:latest
RUN apk update &&\
apk add python3 &&\
apk add py-pip

RUN python3 -m pip install --upgrade pip &&\ 
python3 -m pip install --upgrade dnacentersdk
