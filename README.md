# hosting-static-website-using-docker-compose
Download both the index.html file and Dockerfile and save it in a same directory or folder. 

Go to command prompt and change to the directory where the files are stored. Then, run the command:
docker build -t html .
This commmand helps in building custom image derived from nginx.

After that, we run the command:
docker run -d -p 80:80 html
This command builds a container with the custom image that was just created and the container would operate on port 80 of both the machine and the container.
