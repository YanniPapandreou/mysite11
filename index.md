@def title = "My Franklin Sandbox"
@def hasmath = true
@def hascode = true

# Set up

## Update title

## Update config.md file

* change author
* add site name for GitHub

## Create a table of contents (optional)

\toc

## Upload using GitHub Desktop

# Examples

## How to enter text

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lobortis neque ut ex aliquam, vulputate imperdiet ipsum volutpat. Nunc at mattis eros, eu dapibus nisi. Maecenas commodo tristique cursus. Maecenas pretium, sem et mattis maximus, felis orci ullamcorper ex, quis venenatis risus nisi sit amet velit. Nullam porta sem sed ultricies faucibus. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Phasellus finibus dapibus vehicula. Aenean et tortor eu purus cursus dictum. Mauris eleifend laoreet enim, in facilisis elit tempus et. Sed lobortis tortor vitae augue malesuada, vel tincidunt tortor accumsan. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Vivamus eget ante id eros ullamcorper consequat eget id risus. Ut accumsan odio urna, quis sagittis lorem pretium eu. Proin iaculis massa arcu, in viverra nulla varius vitae. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Fusce malesuada, magna a ultrices accumsan, augue nunc euismod magna, quis luctus eros mauris a nibh. 

## How to render math equations

$$ a^2 + b^2 = c^2 $$

$$ \frac{d}{dx} \int_a^x f(t)dt = f(x) $$

$$ \bar{x} = \frac{1}{n} \Bigg(\sum_{i=1}^n x_i \Bigg) = \frac{x_1 + x_2 + \cdots + x_n}{n} $$

$$ 
  \begin{alignedat}{3}
    2&x + y \space- &z &= &8 \\
    -3&x -y + 2&z &= \space&-11 \\
    -2&x + y + 2&z &= &-3
  \end{alignedat}
$$

$$
  \begin{bmatrix}
    \begin{aligned}
      &2 & &1 & -&1\space \\
      \space -&3 & -&1 & &2 \\
      -&2 & &1 & & 2
    \end{aligned}
  \end{bmatrix}
$$

(optional: disable numbering in `franklin.css` file)

## How to insert Julia code (with outputs!)

Hello, World!

```julia:./ex11
println("Hello, World!")

```

\show{./ex11}

Basic Math

```julia:./ex12
1 + 1
```

\show{./ex12}

Create Function

```julia:./ex13
function add(x, y)
  x + y
end
```

\show{./ex13}


```julia:./ex14
add(2, 3)
```

\show{./ex14}

Random Numbers

```julia:./ex15
rand(5, 5)
```

\show{./ex15}

## How to insert a table from a CSV file

World Population by Region by Year:

\tableinput{}{./tableinput/population_by_year.csv}

@@source
Source: Wikipedia
@@

## How to insert an image file

![beeswarm plot of population by region](/assets/p_beeswarm_region.svg)

@@source
Source: Wikipedia
@@

## How to insert a clickable thumbnail to a YouTube video

[![YT thumbnail](https://img.youtube.com/vi/fVBiLEtZB7A/0.jpg)](https://youtu.be/fVBiLEtZB7A?list=PLhQ2JMBcfAsh5QGVR-DE6qJCGx7CC1OSh)

## How to inject raw HTML

~~~
<iframe width="640" height="360" src="https://www.youtube.com/embed/fVBiLEtZB7A?list=PLhQ2JMBcfAsh5QGVR-DE6qJCGx7CC1OSh" title="[03x09] Intro to Franklin, a Julia Static Site Generator | 9/13 | Julia Web Tools for Beginners" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
~~~


<!-- # Franklin syntax sandbox -->
<!---->
<!-- This page is meant as a sandbox for Franklin Syntax so that you can quickly practice or experience things. -->
<!---->
<!-- ## Sandbox -->
<!---->
<!-- Write whatever you want here to practice Franklin Syntax: -->
<!---->
<!-- ```julia:./ex1 -->
<!-- using LinearAlgebra, Random -->
<!-- Random.seed!(135) -->
<!-- a, b = randn(50), randn(50) -->
<!-- println(dot(a, b)) -->
<!-- println(sum(ai * bi for (ai, bi) ∈ zip(a, b))) -->
<!-- ``` -->
<!---->
<!-- \output{./ex1} -->
<!---->
<!-- (yet another example that floating point arithmetics can be complicated). -->
<!---->
<!-- $$ \forall x \in \R:\quad \scal{x, x} \ge 0 $$ -->
<!---->
<!-- \newcommand{\E}{\mathbb E} -->
<!---->
<!-- Surely some people remember the ordering, but I always forget: -->
<!---->
<!-- $$ \varphi(\E[X]) \le \E[\varphi(X)] $$ -->
<!---->
<!-- for $\varphi$ convex. -->
