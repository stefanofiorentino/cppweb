## docker commit 
cd ~/devel/cppweb

docker cp . 5776c60812d0:/usr/src/cppweb

docker commit 5776c60812d0 hello_crow:latest

## heroku login 
heroku login

heroku container:login

heroku create

docker build -t hello_crow .

heroku container:push web -a evening-garden-48833

heroku container:release web -a  evening-garden-48833

heroku open -a evening-garden-48833

## docker hub
docker login --username=fiorentinoing

docker tag b1f99d016971 fiorentinoing/hello_crow:latest

docker push fiorentinoing/hello_crow

docker pull fiorentinoing/hello_crow

docker rm -f hello_crow_latest

docker run -d -e "PORT=8080" -p 8080:8080 --name hello_crow_latest fiorentinoing/hello_crow

curl -k --silent http://localhost:8080 && echo
