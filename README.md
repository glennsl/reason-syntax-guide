# reason-syntax-guide

This guide aims to quickly answer two questions you might get when you encounter unfamiliar syntax in Reason: What is this And where can I learn more? If it doesn't, please make ~~an issue or~~ a PR.

The guide is divided into these sections
* [Keywords](#keywords)
* [Operators and symbols](#operators-and-symbols)
* [Common user-defined operators](#common-user-defined-operators)
* [Constructs](#constructs)

## Keywords

Keyword          | Usage                    | What is this?                                   | Where can I learn more?
:---             | :---                     | :---                                            | :---
`as`             | `{ foo, bar } as record` | Binds the item being destructured to a name     | [RWO](https://realworldocaml.org/v1/en/html/lists-and-patterns.html#terser-and-faster-patterns) - [OCaml Manual](http://caml.inria.fr/pub/docs/manual-ocaml/patterns.html)
`as`             | `array 'a as 'this`      | A type alias                                    | [OCaml Manual](https://caml.inria.fr/pub/docs/manual-ocaml/types.html#sec97)
`fun`
`let`
`mutable`
`type`
`switch`
`rec`
`in`
`to`
`downto`
`module`
`module type`
`ref`
`true`
`false`
`if`
`else`
`for`
`while`
`open`
`exception`


## Operators and symbols

Operator/Symbol      | Usage                     | What is this?                       | Where can I learn more?
 :---                | :---                      | :---                                | :---
`+.`, `*.`, etc.     | `3.1 +. 2.3`              | Floating point operators            | 
`^`                  | `"Hello " ^ "world"`      | String concatenation                |
`##`                 | `obj##property`           | Object (not record) property access | 
`|>`                 | `"hello" |> print_string` | Pipe operator                       |
`@@`
`=>`    <!-- function, functor, pattern matching -->
`|`     <!-- Variant and pattern separator -->
` ' `   <!-- Type parameter: (`'t`) -->
`` ` `` <!-- Polymorhpic variant: (`` `Thing ``) -->
`::`    <!-- Labeled arguments -->
`{..}`
`...`   <!-- Spread operator, array, object, destructuring -->
`;`
`==`
`===`
`!=`
`!==`
`_`
`land`
`lor`
`lxor`
`lnot`
`lsl`
`lsr`
`not`
`&&`
`||`
`:=`


## Common user-defined operators
`>>=`
`!?`


## Constructs

Syntax                      | Usage                     | What is this?                       | Where can I learn more?
:---                        | :---                      | :---                                | :---
`[<x>, <y>, ...<z>]`        | `let a = [1, 2, ...nums]` | Immutable list append               |
`[<x>, <y>, ...<z>]`        | `let [b, c, rest] = a`    | List destructuring                  |
`type <x> = | <y> | <z>`    |
`fun <x> => ...`            |
`switch <x> { | <y> => ...` |
`{..}`
`{. <x> }`
`{ "<x>": <y> }`
`[| <x>, <y> |]`
`[@@...]` <!-- Attribute -->
`[%...]` <!-- Extension node -->
`/* ...*/`
`<x> ? <y> : <z>`
`(<x>, <y>)` <!-- Tuple -->
`module <X> (<Y>: <Z>) => ...`<!-- Functor -->
`<..>`  <!-- JSX element -->
