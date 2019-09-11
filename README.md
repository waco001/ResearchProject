
# Research Project
## Initial testing of a Python-based AI Scraper. Used in INDEPENDENT RESEARCH IN CYBER SCIENCE SY495. Under instruction of Professor De Bels and Mr. Dias. USNA C/O 2021

 1. create network

    sudo docker network create 495net

 2. mongo container

    sudo docker run --name db -p 27017:27017 --net 495net --mount type=bind,source="/Users/waco001/Desktop/495AI/db/",target="/data/db" mongo

 3. app container

    sudo docker run --name app -p 8080:80 --net 495net 495app
