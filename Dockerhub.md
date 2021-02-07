You either need to tag it as <myuser>/hellodocker when you build it, e g

docker build -t <myuser>/hellodocker:mytag .
or create a new tag tied to the same image, i e

docker tag hellodocker:mytag <myuser>/hellodocker:mytag
and then docker push

docker push <myuser>/hellodocker:mytag
