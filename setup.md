# References
https://itnext.io/setup-flask-project-using-docker-and-gunicorn-4dcaaa829620



# Step 1: Create Docker Image

    Build command, using the terminal, inside the folder that you have your Dockerfile, type: 
    
    docker build -t flask/flask_docker .


    What this command does is use the build command, with the parameter “-t” that specifies that we want Docker to create an image tag name “flask/flask_docker” and the dot “.” is to specify a path where our Dockerfile is, in our case we are in the same folder.


# Step 2: Verify Image

    docker images   


# Step 3: Run Container 

    Run your created container using this command: 

    docker run -d -p 80:80 flask/flask_docker