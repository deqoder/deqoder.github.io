## C89 standard library

### difinition
| sort| header | type           | variable/constant | function |
| --- | ------ | -------------- | ------------------| --------|
| sys | errno  |                | errno                 | |
| sys | stddef |ptrdiff_t,size_t| NULL               | offsetof |
| lang| ctype  |                |              | is(cntrl/print), is(space/graph), is(punct/alnum) <br/> is(digit/xdigit/alpha), (is/to)(lower/upper)|
| lang| locale | struct lconv   |                       | setlocale, localeconv |
| math| limits |                | CHAR_BIT, MB_LEN_MAX <br/> (SCHAR/CHAR/SHRT/INT/LONG)_(MIN/MAX) <br/> U(CHAR/SHRT/INT/LONG)_MAX  | |
| math| float  |                | FLT_RADIX <br/> (FLT/DBL/LDBL)\_(MANT_DIG/DIG/EPSILON/ROUNDS) <br/> (FLT/DBL/LDBL)\_(MIN/MAX)\_(EXP/10_EXP/) | |

### system interface
| sort   |header| type           | variable/constant     | function     |
|--------|------| -------------- | --------------------  | -------------|
| cpu    |setjmp| jmp_buf        |                       | setjmp longjmp |
| cpu    |signal| sig_atomic_t   |SIG(FPE/ILL/SEGV), SIG(ABRT/INT/TERM)| signal, raise, SIG_(DFL/IGN/ERR) |
| cpu    |assert|                |                       |  assert |
| mem&cpu|stdlib| div_t, ldiv_t, size_t |  (MB_CUR/RAND)\_MAX <br/> EXIT\_(FAILURE/SUCCESS), NULL                     | (m/c)alloc/free, ato(i/f), strto(d) |
| io     |stdio | FILE, fpos_t, size_t |  BUFSIZ, (FILENAME/TMP/FOPEN)\_MAX, L_tmpnam <br/> std(in/out/err), EOF, NULL, SEEK_(CUR/END/SET), _IO(F/L/N)BF | (v)(s/f)(print/scan)f, (f)(put/get)(char/c/s), f(read/write) | 
| time   | time | time_t, clock_t, struct tm <br/> size_t |  CLOCKS_PER_SEC <br/> NULL  | time, clock, difftime, (local/gm/mk)time <br/> (asc/c/strf)time |

### utils
| sort| header | type   | variable/constant| function           |
| ----| ------ | ------ | -----------------| ------------------ |
| sys | stdarg | va_list|                  | va_(start/end/arg) |
| lang| string | size_t |  NULL            |                    |
| math|  math  |        | NAN, HUGE_VAL    | (/(a)(sin/cons/tan)(h), atan2|
