# CS61: Lecture 10

### assembly

#### attackme.unsafe.s
- rough size of local variables being allocated on stack: 112 bytes
.. - likely takes exactly one arg
- copying string one character at a time into local sotrage
- checksum
.. - fixed length summary of a varaible length array 


#### hashcode
```c++
hashcode(std::string)
```
-returns object of size_t
- properties:
.. 1. **mandatory** if x1 == x2, then hashcode(x1) == hashcode(x2)
.. 2. **desirable** if x1 != hx, then hashcode(x1) != hashcode(x2)


#### return to libc attack
- need to know where the address of the libc function is
- can be prevented by stack checking


### storage
- **cache** -> small amount of fast storage used to speed up access to larger, slower storage
-  everytime you want to change any part of the state of a flashdrive you need to change 64KB of the flashdrive
.. - changes committed in flash blocks
- **buffer cache** -> cache of primary memory used to speed up access to disks
.. - can hold multiple files worth of data
- **kernal**
.. - kernal calls very expensive

#### storage1
- ./w01
- everytime one byte is being written on program side travels through operating system and comes out as 64KB of changes to the mechanical drive
- could the operating system improve its performance?
.. 1. could use buffer cache to make significantly faster
.... - ./w03-byte
.... - makes it about 348 times faster



```c++
for (int i = 0; i < 10; i++){
	printf("%i\n", i);
}
```
```c++
for (int i = 0; i < 10; i++){
	printf("%i\n", i);
}
```
**this is bold**
