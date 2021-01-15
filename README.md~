# Simple PHP File Hash Calculator

## Build
docker build -t php-hash .

## Run
docker run -p 8080:80 -dt php-hash

## Test

##### Default hash is md5
curl -F "file=@Dockerfile" localhost:8080
##### Response
93f835e70e90ff70de7f0ac721072185tmps

##### Pass specific hash
curl -F "algo=sha256" -F "file=@/path/to/file" localhost:8080
##### Response
f40e9648703a92954f1dc02534a22529d3b0e705aab87253a0e54bff4ed28e67tmps
