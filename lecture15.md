# Lecture Note 221 - L15

## Structures

### Linked List Example {1.1}

Since the compiler only understands the size and index we determine it using the memory pointer method {?} <br>
The method we will be using to determine the information is to point to the $Contiguous Memory$<br>

![image](https://github.com/MaxHao56/2023-Documentaton/assets/132418186/07173cd0-8fc9-496d-94bf-bece29de4b71)<br>

`Structure` - Block of Memory  &rarr; Computes with Equation `r + 4*i`<br>

<br>
<br>


### Unalignment of Structure {1.2}

This is to determine the size of the $Contiguous Memory$<br>

`Addition` is the way to go <br>

This chart below indicates the size of different types of data

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

<br>
<br>

### Alignment of Structure {1.3}

The Alignment fills $Gaps$<br>
The Alignment Takes the Largest Type of Bytes(K) And points using the $K*$<br>

![image](https://github.com/MaxHao56/2023-Documentaton/assets/132418186/5132077f-5fd7-4d22-a29e-e1ebbc622def)<br>
![image](https://github.com/MaxHao56/2023-Documentaton/assets/132418186/be9f5934-5c27-43dc-9260-ae98f87d581b)<br>

This shows how it stores each line in the struct<br>
An array of the struct is struct followed by an array with index &rarr; r + K*i`<br>

Saving Space by putting large data types first

<br>
<br> 

## Unions

Unions don't have to fill the largest type of memory. <br>
They still use the largest memory to define `final size` <br>
But they don't fill gaps easily. They use as much space as they can. <br>
![image](https://github.com/MaxHao56/2023-Doc/assets/132418186/d24b334c-c29f-4a69-97d9-9b5dd0bb637a) <br>


## Floating Point

They are 16 bytes = 256 bits <br>
`Single Precision` = 4 bytes = uses %mm1 and %mm0 as input to generate %mm0 <br>
`Double Precision` = 8 bytes = uses %mm1 and %mm0 as input to generate %mm0 <br>

![image](https://github.com/MaxHao56/2023-Doc/assets/132418186/4c599da5-93aa-4510-aa79-3aa4800f652f)




floating point has 256 bits meaning 32 bytes and 128 as part of it![Alt text](image-1.png)
