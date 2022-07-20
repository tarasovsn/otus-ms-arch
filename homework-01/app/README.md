Build fat jar:

    mvn package

Build docker image:

    docker build . -t tarasovsn/health-img:0.0.1

For Mac M1 BUILD command add this flag:

    --platform=linux/amd64

Run container:

    docker run -d -p 80:8000 --name health tarasovsn/health-img:0.0.1

Push image to Docker Hub:

    docker image push tarasovsn/health-img:0.0.1