---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default 
---

I am a doctoral student in the High Performance Computational Physics group
under the supervision of Prof. Dr. Marina Marinkovic, where I develop
and implement algorithms for the simulation of particle physics.

Previously, I worked as a software engineer at Embotech implementing
algorithms for automotive motion planning. Before that, I completed
my Master and Bachelor degree in Physics at ETH Zürich.

# Projects

Here are some of the projects that I have recently worked on.

### Inverse trace estimation of sparse matrices

The calculation of the trace of an inverse of a matrix 
requires solving a linear system of equations n times, with n the
dimension of the matrix. This becomes quickly infeasible for large dimensions.
In this project, I implemented a stochastic estimate for the trace that exploits
the sparsity of the given matrix. 

The code was written in the C language
with extensive use of MPI, and ran on both CPU and GPU clusters
by CSCS. It is integrated into the 
[rcstar/openQxD-devel](gitlab.com/rcstar/openQxD-devel) code package;
see [rcstar/openQxD](gitlab.com/rcstar/openQxD)
for a public version of the repository.

### Real-linear operators

The use of conjugation boundary conditions, needed for simulating quantum electrodynamical
effects, changes the equations that govern the dynamics of physics from linear operator
to real-linear operators of the form f(v) = Av + Bv*. In this project,
we investigate the inversion of such maps. 

It is written in modern C++
and publicly available on [donion74/cstar-bc](https://gitlab.com/donion74/cstar-bc).

### Optimization on manifolds, semidefinite programming

Quantum resources bear the potential for higher precision on measurements
than their classical counterpart. In this project, we formulated the optimal
measurement strategy as an optimization problem over a space of positive
semidefinite matrices and solved it using semidefinite programming.
Due to the exponential scaling with respect to the number of resources,
we then formulated an approximate solution that performs a minimization over
a manifold of matrices.

The first part of the project is written in Matlab and publicly available
under [donion74/comb-estimation](https://gitlab.com/donion74/comb-estimation).
The second part of the project is written Python and uses tensorflow to
implement a gradient descent algorithm, it is available
under [donion74/comb-efficient](https://gitlab.com/donion74/comb-efficient).


### Optimization algorithms for automotive applications

Motion planning in autonomous vehicle requires real-time decision making
in a reliable and efficient manner. To increase the speed of solving
the corresponding dynamics equation, I implemented an implicit 
differential equation solver while propagating the gradient with
respect to initial parameters.

The code was integrated into the [FORCESPRO](https://embotech.com/forcespro)
package by Embotech, has achieved 2-10x speedups and has been used by 
customers and employees alike.

### Exam translation, printing and scanning

The organization of international scientific Olympiads such as IPhO, IBO
or IChO, require the translation of the original English exam into
over 90 languages within a short amount of time. The coordination 
is greatly facilitated by our organization [OlyExams](https://oly-exams.org/).

As part of this organization, I maintain the publicly available
[exam_tools](https://gitlab.com/oly-exams/exam_tools),
written in Python and with Django, 
have instructed local organizing committees and deployed at events
in Israel, Armenia, and UAE.


# Coursework

In the course of my education, I have built a solid foundation in physics,
mathematics and computer engineering. Here are some of the recent courses I followed.

### Compiler Design

This course is offered in the 3rd year of the computer science bachelor at ETH Zürich
and introduces lexical analysis, top-down and bottom-up parsing, abstract syntax trees,
intermediate representations. I completed assignments in OCaml that transforms
Oat programs via LLVM and x86 Assembly to byte code.

### Computer Systems

This course is offered in the 3rd year of the computer science bachelor 
at ETH Zürich. I followed the first half of the lecture, which introduces
scheduling, operating system structures, interprocess communication, memory
management and file systems.

### Systems Programming and Computer Architecture

This course is offered in the 2nd year of the computer science bachelor 
at ETH Zürich and introduces hardware features like exceptions, interrupts,
caches, virtual memory and devices. I completed practical assignments
in the C language and x86 Assembly.

### Functional Programming

This course is offered in the 2nd year of the computer science bachelor 
at ETH Zürich and introduces the lambda calculus, higher-order programming and proofs of correctness. Practical assignments were carried out in Haskell.

### Communication Networks

This course is offered in the 3rd year of the electrical engineering bachelor 
at ETH Zürich and introduces the protocol layers of networks.
Practical assignments included operating a mini-internet that involved
setting up OSPF, BGP and VPN configurations, and
implementing a TCP-like reliable transport protocol.

### Finite Element Methods

This course if offered in the computational science bachelor at ETH Zürich
and introduces finite element methods to solve partial differential
equations. A large part of the course consisted in completing 
assignments in C++ in the [LehrFEM++](https://github.com/craffael/lehrfempp)
package.


<!-- Text can be **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](./another-page.html).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# Header 1

This is a normal paragraph following a header. GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

## Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
``` -->

