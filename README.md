#Shellcoding
To disable ASLR:

    sudo bash -c 'echo 0 > /proc/sys/kernel/randomize_va_space'

To disable stack canaries

    gcc overflow.c -o overflow.out -fno-stack-protector
