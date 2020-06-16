# django-web01

## Build Image
git clone https://github.com/zhenjunz/django-web01.git
cd django-web01
docker build -t *.*.*.59:9005/django-web01:master .
docker push *.*.*.59:9005/django-web01:master

## Start Container
docker run -d -p 8081:8000 --name mydjango *.*.*.59:5000/django-web01:master
curl localhost:8081

## Deploy
https://blog.csdn.net/xujiamin0022016/article/details/104686997/