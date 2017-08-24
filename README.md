# Container Intro

## Introduction to containers with a simple python app.

```bash
$ git clone https://github.com/grafuls/container-intro.git
$ cd container-intro
$ docker build -t hellopython .
$ docker run -p 4000:80 hellopython
```

- You should see a notice that Python is serving your app at http://0.0.0.0:80. But that message is coming from inside the container, which doesn’t know you mapped port 80 of that container to 4000, making the correct URL http://localhost:4000.
