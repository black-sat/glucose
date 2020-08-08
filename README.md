# The Glucose SAT Solver

Glucose is based on a new scoring scheme (well, not so new now, it was
introduced in 2009) for the clause learning mechanism of so called "Modern" SAT
solvers (it is based our IJCAI'09 paper). It is designed to be parallel, since
2014. This page summarizes the techniques embedded in all the versions of
glucose. The name of the Solver name is a contraction of the concept of "glue
clauses", a particular kind of clauses that glucose detects and preserves during
search. Glucose is heavily based on Minisat, so please do cite Minisat also if
you want to cite Glucose.

-- [Gilles Audemard](http://www.cril.fr/~audemard/) and [Laurent Simon](http://www.labri.fr/perso/lsimon/)

# Directory overview:
 
| Item          | Description               
|---------------|------------------------------------------------------
| mtl/          |  Minisat Template Library
| core/         |  A core version of the solver glucose (no main here)
| simp/         |  An extended solver with simplification capabilities
| parallel/     |  A multicore version of glucose
| README        |  
| LICENSE       |
| Changelog     |

# To build (release version: without assertions, statically linked, etc):
Like minisat....

cd { simp | parallel }
make rs

# Usage:

in simp directory:      ./glucose --help

in parallel directory:  ./glucose-syrup --help