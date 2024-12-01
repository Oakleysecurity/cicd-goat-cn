FROM gitlab:5050/wonderland/nest-of-gold/python:3.8

WORKDIR /app
COPY app.py .
COPY requirements.txt .
RUN pip3 install -r requirements.txt -i http://pypi.douban.com/simple --trusted-host pypi.douban.com

CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0"]
