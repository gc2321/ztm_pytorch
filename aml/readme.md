## Build Image
```
docker build -t pytorch-cuda .
```

## Run Container

```
docker run --gpus all -p 8888:8888 -it \
  -v C:\\Users\\kaizi\\Desktop\\jupyter\\aml:/app/notebooks \
  -v C:\\Users\\kaizi\\Desktop\\jupyter\\aml\\aml_data:/app/data \
  --name pytorch-cuda-container pytorch-cuda
```

## start container

```
docker start -ai [containerID]
```