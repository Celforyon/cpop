# CPOP

A container with what is required to compile CPOP

## Usage
```bash
docker run --rm -it -e CWD=$(pwd) -v $(pwd):$(pwd):rw celforyon/cpop
```

Once in the container, you can do as usual:
```bash
mkdir build
cd build
cmake ..
make
```

### In case user ID is not 1000
```bash
docker run --rm -it -e USER_ID=${UID} -e CWD=$(pwd) -v $(pwd):$(pwd):rw celforyon/cpop
```
