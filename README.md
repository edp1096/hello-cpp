https://www.joinc.co.kr/w/Site/C/Documents/Make_Library

```sh
cd mysum
gcc -c mysum.c
ar rc libmysum.a mysum.o
cp libmysum.a ../

cd ..
gcc -o print_sum print_num.c -L./ -lmysum
```