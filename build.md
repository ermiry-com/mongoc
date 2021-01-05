# Build Mongo C Driver Docker Images

## Development

Build development image
- Mongo C driver with Debug flags
- Output from ubuntu and gdb installed

```
sudo docker build -t ermiry/mongoc:development -f Dockerfile.dev .
```

## Development Builder

Build development builder image
- Mongo C driver with Debug flags
- Output from gcc and gdb installed

```
sudo docker build -t ermiry/mongoc:buildev -f Dockerfile.buildev .
```

## Builder

Build builder image
- Mongo C driver with Release flags
- Output from gcc and without gdb

```
sudo docker build -t ermiry/mongoc:builder -f Dockerfile.builder .
```

## Production

Build production image
- Mongo C driver with Release flags
- Output from ubuntu and without gdb

```
sudo docker build -t ermiry/mongoc:latest -f Dockerfile .
```