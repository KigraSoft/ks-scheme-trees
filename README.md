# KigraSoft Scheme Trees

Scheme Trees is the start of a library to implement various k-ary
trees for use in Scheme programs.  I was working on a scheme project
and it seemed like some of the data structures would be best
implemented using some sort of binary search tree.  Since multiple
data structures would benefit, building the capability in a libary
seemed the best approach.  Not sure yet if this will even do what I
want, but it is offered here for anyone that might find it useful.

## Tree Structures Implemented

So far only a basic unbalanced binary search tree (BST) is implemented
(and not completely yet).  The intent is to also implement some 
self-balancing binary trees and a B-tree structure.  The intent is to
do so in a way that the tree structure type is selected at
initialization and then the underlying structure is not relevant to
its use after that.

## Usage

Three functions are available so far:

- (make)
  Returns an empty BST structure

- (insert bst key datum)
  Insert a datum into an initialized bst using key for its index

- (print bst)
  Print a rough tree graph of bst for diagnostic purposes

## Implementation

The code is currently being develop in a literate style using Emacs Org-mode.

To extract the code, load it into Emacs and run M-x org-babel-tangle
(C-c C-v t) to generate Guile Scheme code.

## Compatibility

The code is intended to be R7RS compliant with SRFI libraries as
needed.  So far it is only being tested in Guile Scheme 3.10 and so
there may be some Guile specific code that has crept in.

