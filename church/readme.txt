church encoding ruleset for mlatu
inspired by https://www.youtube.com/watch?v=TcveznrwYtk

here, a church-encoded value V is the first class quote, and to invoke it, you need V<
in joy's schemes, a data type V is a function, NOT a quote, meaning that V would invoke it, and (V) would represent the first class version
here is a handy table that I made:
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
language:  | style:  | call with arg x: | pass to function f:
mlatu      | postfix | x V<             | V f
joy-like   | postfix | x V              | (V) f
LC/CL      | prefix  | V x              | f V
lisp       | prefix  | (V x)            | (f V)
imperative | prefix  | V(x)             | f(V)