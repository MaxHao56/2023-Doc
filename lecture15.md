everything works as memory like linked list
with formula of r + 4\*i and r starts at the starting point and i is the index of the list

later with structures & alignment with
`unaligned data ` =![image](https://github.com/MaxHao56/2023-Documentaton/assets/132418186/176bc245-f275-48e5-9d66-acbeff1368cd)

we use better alignment to use to find the memeory

meaning if int = 4 then => then it should start or land on at the mutiple of 4 meaning 4k

so there is initutive way and there is alignment way [noalign][align]

| Data Type      | Size (in bytes) on a 64-bit System |
| -------------- | ---------------------------------- |
| char           | 1                                  |
| unsigned char  | 1                                  |
| int8_t         | 1                                  |
| short          | 2                                  |
| unsigned short | 2                                  |
| int16_t        | 2                                  |
| int            | 4                                  |
| unsigned int   | 4                                  |
| int32_t        | 4                                  |
| long           | 8                                  |
| unsigned long  | 8                                  |
| int64_t        | 8                                  |
| float          | 4                                  |
| double         | 8                                  |
| long double    | 16                                 |
| pointers       | 8 (on most 64-bit systems)         |
| structures     | Size depends on the members        |
| arrays         | Size depends on element type and   |
|                | number of elements                 |

for alignment find the largest of alignment byte = K and have to be mutiple of K

insert gaps if needed

alignment is more effcient

each part of the struct is the K\* of the largest

with alignment you can't count you have to follow the equation and use the formula to find otherwise you will get lost
above is the struct and we have union = strucut have different element but all can have different tyeps

union only store same data types in each section![Alt text](image.png)

union doesn't have gaps ; structs have gaps

floating Point registers
floating point has 256 bits meaning 32 bytes and 128 as part of it![Alt text](image-1.png)
different precsion takes into the place
is how the add together to become the 256 bits
and their arguments gets passed and results get return
