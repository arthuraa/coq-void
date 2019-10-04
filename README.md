# Coq Void

The MathComp library has instances for most basic Coq types, but it leaves out
`Empty_set`.  This library simply defines a `void` alias for that type, as well
as `eqType`, `choiceType`, `countType` and `finType` instances.

## Requirements

The library has been tested with the following versions, but probably works with
older ones as well.

- Coq 8.9

- `coq-mathcomp-ssreflect` 1.9

## Usage

To compile, do

    coq_makefile -f _CoqProject -o Makefile
    make
    make install

You can import the library with

    From void Require Import void.
