# my-small-app

A minimal Angular v21 single-page application featuring a click counter. Built with standalone components and served via nginx inside a Docker container.

**Live app:** https://my-small-app.onrender.com

## Run

```bash
docker run -p 8080:80 andrewzlobin/my-small-app
```

Then open [http://localhost:8080](http://localhost:8080) in your browser.

## Build locally

```bash
# Clone / download the source, then from the project directory:
docker build -t andrewzlobin/my-small-app .
docker run -p 8080:80 andrewzlobin/my-small-app
```

## Stack

- Angular 21 (standalone components)
- nginx:alpine (serves the production build)
- Multi-stage Docker build — final image is ~50 MB
