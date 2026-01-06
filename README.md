# assembly
program that converts this symbolic representation into machine code ready to be executed by a CPU is called an Assembler and to examine the state of the code we would be using an Debugger

cpu follows a set of instructions
<img width="1024" height="768" alt="image" src="https://github.com/user-attachments/assets/71f7be93-8e48-4d91-b497-01d998076523" />

cpu contains registers, each of them are 64 bit wide, and for each of them the lower byte, word and double-word can be addressed. for ex: 1 "word" = 2 bytes, 1 "double-word" = 4 bytes

Register	Lower byte	Lower word	Lower dword
rax	al	ax	eax
rbx	bl	bx	ebx
rcx	cl	cx	ecx
rdx	dl	dx	edx
rsp	spl	sp	esp
rsi	sil	si	esi
rdi	dil	di	edi
rbp	bpl	bp	ebp
r8	r8b	r8w	r8d
r9	r9b	r9w	r9d
r10	r10b	r10w	r10d
r11	r11b	r11w	r11d
r12	r12b	r12w	r12d
r13	r13b	r13w	r13d
r14	r14b	r14w	r14d
r15	r15b	r15w	r15d

Additionally, the higher 8 bits of rax, rbx, rcx and rdx can be referred to as ah, bh, ch and dh.

rsp holds the stack pointer (which is used by instructions like push, pop, call and ret), and rsi and rdi serve as source and destination index for "string manipulation" instructions

rip and rflags. rip holds the address of the next instruction to execute. 
modified by control flow instructions like call or jmp. 
rflags holds a bunch of binary flags indicating various aspects of the program's state, such as whether the result of the last arithmetic operation was less, equal or greater than zero.
