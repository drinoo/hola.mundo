.section .data

	msj: .asciz “esta es la tarea de orga”.section.text

.globl main
main:

	pushl $msj
	call printf
	addl $4, %esp

	movl $1, %eax
	movl $0, %ebx
	int $0x80
