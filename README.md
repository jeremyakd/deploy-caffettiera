# deploy-caffettiera
Repo para deployar nuestra web  
  
docker login  
docker-compose pull  
docker-compose -f docker-compose.yml up -d  


# Pasos para buildear la imagen

docker build --tag web_caffettiera:1.0.0 .  
docker tag web_caffettiera:1.0.0 <user>/mirepo:1.0.0  
docker login  
docker push <user>/mirepo:1.0.0  