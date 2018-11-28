## C89 standard library

| sort                          | header | type           | variable/constant     | function |
|------------------------------ |------- | -------------- | --------------------  | -------- |
| define int                    | limits |                |                       | |
| define float                  | float  |                |                       | |
| define char                   | ctype  |                |                       | |
| define exception code         | errno  |                |                       | |
| define string                 | locale |                |                       | |
| define                        | stddef |                |                       | |
| system/io & strconv           | stdio  | FILE           | stdin, stdout, stderr | (v)(s/f)(print/scan)f, (f)(put/get)(char/c/s), f(read/write) | 
| system/memory & strconv & math| stdlib |                |                       | (m/c)alloc/free, ato(i/f), strto(d) |
| system/cpu                    | setjmp |                |                       | |
| system/cpu                    | signal |                |                       | |
| system/cpu                    | assert |                |                       | |
| system/time                   |  time  | time_t clock_t |                       | time, asctime, ctime |
| library/string                | string |                |                       | |
| library/syntax sugar          | stdarg |                |                       | |
| library/math                  |  math  |                |                       | |
