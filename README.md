# Simple PHP File Hash Calculator

## Build
docker build -t php-hash .

## Run
docker run -p 8080:80 -dt php-hash

## Test

#### Default hash is md5
curl -F "file=@/path/to/file" localhost:8080
#### Response
93f835e70e90ff70de7f0ac721072185

#### Pass specific hash
curl -F "algo=sha256" -F "file=@/path/to/file" localhost:8080
#### Response
f40e9648703a92954f1dc02534a22529d3b0e705aab87253a0e54bff4ed28e67

#### Algorithms
Array
(
    [0] => md4
    [1] => md5
    [2] => sha1
    [3] => sha256
    [4] => sha384
    [5] => sha512
    [6] => ripemd128
    [7] => ripemd160
    [8] => whirlpool
    [9] => tiger128,3
    [10] => tiger160,3
    [11] => tiger192,3
    [12] => tiger128,4
    [13] => tiger160,4
    [14] => tiger192,4
    [15] => snefru
    [16] => gost
    [17] => adler32
    [18] => crc32
    [19] => crc32b
    [20] => haval128,3
    [21] => haval160,3
    [22] => haval192,3
    [23] => haval224,3
    [24] => haval256,3
    [25] => haval128,4
    [26] => haval160,4
    [27] => haval192,4
    [28] => haval224,4
    [29] => haval256,4
    [30] => haval128,5
    [31] => haval160,5
    [32] => haval192,5
    [33] => haval224,5
    [34] => haval256,5
)

