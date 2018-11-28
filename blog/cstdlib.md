## C89 standard library

| sort                          | header | type           | variable/constant     | function |
|------------------------------ |------- | -------------- | --------------------  | -------- |
| define/int                    | limits |                |                       | |
| define/float                  | float  |                |                       | |
| define/char                   | ctype  |                |                       | |
| define/exception code         | errno  |                |                       | |
| define/string                 | locale |                |                       | |
| define                        | stddef |                |                       | |
| system/cpu                    | setjmp | jmp_buf        |                       | setjmp longjmp |
| system/cpu                    | signal | sig_atomic_t   |SIG(ABRT/FPE/ILL/INT/SEGV/TERM)| signal, raise, SIG_(DFL/IGN/ERR) |
| system/cpu                    | assert |                |                       |  assert |
| system/memory & strconv & math| stdlib |                |                       | (m/c)alloc/free, ato(i/f), strto(d) |
| system/io & strconv           | stdio  | FILE           | stdin, stdout, stderr | (v)(s/f)(print/scan)f, (f)(put/get)(char/c/s), f(read/write) | 
| system/time                   |  time  | time_t clock_t |                       | time, asctime, ctime |
| library/syntax sugar          | stdarg |                |                       | |
| library/string                | string |                |                       | |
| library/math                  |  math  |                |                       | |
