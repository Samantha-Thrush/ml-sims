Run docker with:

vim Dockerfile

sudo docker build -t ipytheano .

sudo docker ps       (gives docker name)

sudo dockerrm -f ________________   (docker name)

sudo docker run -d -p 443:8888 -e "PASSWORD=temp123" -v ~/ml-sims:/notebooks/ml-sims ipytheano
