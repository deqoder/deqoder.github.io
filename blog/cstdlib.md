## C89 standard library

### difinition

| sort| header | type           | variable/constant | function |
| --- | ------ | -------------- | ------------------| --------|
| sys | errno  |                | errno             | |
| sys | stddef |ptrdiff_t,size_t| NULL              | offsetof |
| lang| ctype  |                |     | is(cntrl/print), is(space/graph), is(punct/alnum) <br/> is(digit/xdigit/alpha), (is/to)(lower/upper)|
| lang| locale | struct lconv   | LC_(ALL/COLLATE/CTYPE/MONETARY/NUMERIC/TIME)    | setlocale, localeconv |
| math| limits |                | CHAR_BIT <br/> (SCHAR/CHAR/SHRT/INT/LONG)_(MIN/MAX) <br/> U(CHAR/SHRT/INT/LONG)_MAX  | |
| math| float  |                | FLT_RADIX <br/> (FLT/DBL/LDBL)\_(MANT_DIG/DIG/EPSILON/ROUNDS) <br/> (FLT/DBL/LDBL)\_(MIN/MAX)\_(EXP/10_EXP/) | |

### system interface

| sort   |header| type           | variable/constant     | function     |
|--------|------| -------------- | --------------------  | -------------|
| cpu    |setjmp| jmp_buf        |                       | setjmp, longjmp |
| cpu    |signal| sig_atomic_t   |SIG(FPE/ILL/SEGV) <br/> SIG(ABRT/INT/TERM)| signal, raise<br/> SIG_(DFL/IGN/ERR) |
| cpu    |assert|                |                       |  assert |
| mem<br/>&cpu<br/>&math<br/>&lang|stdlib| (l)div_t<br/>size_t |  EXIT\_(FAILURE/SUCCESS) <br/> RAND\_MAX <br/>  NULL  | (m/c/re)alloc/free <br/> abort/(at)exit, getenv, system <br/> ato(i/l/f), strto(ul/l/d) <br/> (l)(abs/div), (s)rand, qsort/bsearch |
| io     |stdio | FILE<br/>fpos_t<br/>size_t |  (FILENAME/FOPEN)\_MAX, <br/> BUFSIZ, \_IO(F/L/N)BF <br/> SEEK\_(CUR/END/SET), EOF <br/> std(in/out/err)  <br/> L_tmpnam, TMP_MAX, NULL | f((re)open/close) <br/> fflush, set(v)buf <br/> f(get/set)pos, f(tell/seek/eof), rewind <br/> f(read/write), (f)(get/put)(c/s/char), ungetc <br/> (v)(f/s)(print/scan)f, <br/> re(move/name), tmp(file/nam),(f/p)error, clearerr | 
| time   | time | clock_t <br/> time_t<br/>struct tm <br/> size_t |  CLOCKS_PER_SEC <br/> NULL  | clock <br/> time, difftime <br/> (local/gm/mk)time <br/> (asc/c/strf)time |

### utils

| sort| header | type   | variable/constant| function           |
| ----| ------ | ------ | -----------------| ------------------ |
| sys | stdarg | va_list|                  | va_(start/end/arg) |
| lang| string | size_t |  NULL            | memchr, str((r)chr/(c)spn/pbrk/str) <br/> mem(cpy/move), str(n)(cpy/cat) <br/> memcmp, str((n)cmp/coll) <br/> str(xfrm/len/tok/error), memset |
| math|  math  |        | NAN, HUGE_VAL    | f(abs/mod), ceil/floor, modf <br/> pow/sqrt, (fr/ld)exp, log(10) <br/> (a)(sin/cons/tan)(h), atan2|
