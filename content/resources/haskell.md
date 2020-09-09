+++
title = "Haskell"
date = 2020-06-20
+++

# Haskell

[Haskell](https://www.haskell.org/) is an advanced, purely functional programming language with [Hindley-Milner type system](https://en.wikipedia.org/wiki/Hindley%E2%80%93Milner_type_system), concurrent runtime and lazy (non-strict) evaluation.

Things to keep in mind:
- Static type system doesn't necessarily mean wrestling with types like in C thanks to the advanced type inference in Haskell: in fact on many occassions you can let the compiler write your logic for you based on the type signatures
- Lazy evaluation is much more aligned with mathematical reasoning and abstractions: it allows for e.g. manipulations on infinite lists
- One of the defining features of purely functional languages, _referential transparency_, lets us reason about our programs in a much more structured way
- What's more, Haskell programs are, to an extent, provable: you can prove things like [termination](https://en.wikipedia.org/wiki/Termination_analysis) or even correctness of algorithm implementation, see [Curry-Howard correspondence](https://en.wikipedia.org/wiki/Curry%E2%80%93Howard_correspondence)
- That said, Haskell flexibility prevents it from having some of the critical capabilities required to be a fully operational proof assistant like [Coq](https://coq.inria.fr/): it's a trade-off
- Haskell carries deep ideas applicable to modern imperative dynamically typed languages (such as Python): it just might make you a better programmer (but you don't have to program to learn Haskell!)

Format I have in mind is to focus on [LYAH](http://learnyouahaskell.com/chapters) (one chapter per week) and supplement with exercises and relevant chapters from [HFFP](http://haskellbook.com/). During weekly meetings we would then discuss our reflections on the chapter, things we found hard or interesting, go through the solutions for exercises and review relevant blogposts to a level of detail dependent on time constraints.

It would be also great to try and connect what we learn here to our university curriculum, especially MA211 and MA203.

Below you'll find a long list of links, loosely partitioned into vague categories. Have a look and skim a couple pages to get an overall feeling for Haskell. Bold font means it's quality content.

## Motivation

* [**Why Functional Programming Matters**](http://www.cse.chalmers.se/~rjmh/Papers/whyfp.pdf)
* [**Why Haskell Matters**](https://wiki.haskell.org/Why_Haskell_matters)
* [**What is Good About Haskell?**](https://doisinkidney.com/posts/2019-10-02-what-is-good-about-haskell.html)
* [Galois testimony](http://homepages.inf.ed.ac.uk/wadler/realworld/galois.html)
* [**Haskell <-> Mathematics**](https://wiki.haskell.org/Blog_articles/Mathematics)
* [Comparison with other functional languages](http://matt.might.net/articles/best-programming-languages/)
* [Why is Haskell so fast?](https://stackoverflow.com/a/35038374)
* [**Haskell Fan Site**](http://www-cs-students.stanford.edu/~blynn/haskell/)
* [A Brief Guide to A Few Algebraic Structures](https://argumatronic.com//posts/2019-06-21-algebra-cheatsheet.html)
* [**Eleven Reasons to use Haskell as a Mathematician**](http://blog.sigfpe.com/2006/01/eleven-reasons-to-use-haskell-as.html?m=1)
* [Phrasebook (a  fairly cute starting point)](https://typeclasses.com/phrasebook)
* [Writing fast Haskell code (old, but quality showcase)](https://github.com/bitemyapp/learnhaskell/blob/master/write_haskell_as_fast_as_c.md)

## Formal verification and type theory
* [Proving things in Haskell](https://blog.madsbuch.com/proving-stuff-in-haskell/)
* [**Can Haskell be proved?**](https://stackoverflow.com/questions/4077970/can-haskell-functions-be-proved-model-checked-verified-with-correctness-properti)
* [Verifying Haskell Programs by Combining Testing and Proving](http://www.cse.chalmers.se/~peterd/papers/Dallas.pdf)
* [Writing Haskell with Coq](https://www.cs.purdue.edu/homes/bendy/Fiat/FiatByteString.pdf)
* [A Primer on Type Systems](https://www.cs.uaf.edu/users/chappell/public_html/class/2018_spr/cs331/docs/types_primer.html)
* [**What To Know Before Debating Type Systems**](https://cdsmith.wordpress.com/2011/01/09/an-old-article-i-wrote/)
* [Attractive Types](http://okmij.org/ftp/Haskell/types.html)
* [Implement With Types, Not Your Brain!](https://reasonablypolymorphic.com/blog/typeholes/index.html)

## Fundamental resources
* [**Learn You a Haskell for Great Good!**](http://learnyouahaskell.com/chapters) - introductory, easy to follow book, some people with strong opinions fiercely advise against it due to the supposed "illusion of learning" - imho not true
* [**Haskell Programming from First Principles**](http://haskellbook.com/) - modern and comprahensive source, regarded as the best book by far, imho it's way too overrated and doesn't explain things as well as people say it does
* [Real World Haskell](http://book.realworldhaskell.org/read/) - pool of relevant, real-world application-oriented examples
* [How To Organize a Picnic on a Computer](http://lisperati.com/haskell/ht1.html) - engaging tutorial on Haskell thought process
* [What I Wish I Knew When Learning Haskell](http://dev.stephendiehl.com/hask/)
* [Usefull functions in Prelude.hs](https://www.cse.unsw.edu.au/~en1000/haskell/inbuilt.html)
* [Typeclassopedia](https://wiki.haskell.org/Typeclassopedia)
* [Haskell Programming Tips](https://wiki.haskell.org/Haskell_programming_tips)
* [Hitchhikers' Guide to Haskell](https://wiki.haskell.org/Hitchhikers_guide_to_Haskell)
* [Functors, Applicatives, And Monads In Pictures](http://adit.io/posts/2013-04-17-functors,_applicatives,_and_monads_in_pictures.html)
* [H-99: Ninety-Nine Haskell Problems](https://wiki.haskell.org/H-99:_Ninety-Nine_Haskell_Problems)

## Advanced resources
* [**Oleg Kiselyov**](http://okmij.org/ftp/)
* [_Useful Idioms that will blow your mind_](https://wiki.haskell.org/Blow_your_mind)
* [Category Theory for Programmers](https://bartoszmilewski.com/2014/10/28/category-theory-for-programmers-the-preface/)
* [Haskell Symposium](https://www.haskell.org/haskell-symposium/)
* [Creative uses of monads](https://stackoverflow.com/questions/412929/creative-uses-of-monads)
* [Twelve Monads of Christmas](https://medium.com/twelve-days-of-monad)

## Environment
* [General setup in details](https://caiorss.github.io/Functional-Programming/haskell/Haskell.html)
* [Dockerizing Haskell](https://mmhaskell.com/blog/2018/4/25/dockerizing-our-haskell-app)
* [Neovim setup](https://blog.jez.io/haskell-development-with-neovim/)
* [Vim setup](http://www.stephendiehl.com/posts/vim_2016.html)

## Miscellaneous
* [Notes for first year Computing at Imperial College London](https://github.com/jordanspooner/ic-first-year-notes)
* [Lobsters search query](https://lobste.rs/search?utf8=%E2%9C%93&q=haskell&what=stories&order=relevance)
* [What a Haskell Study Group is Not](https://bitemyapp.com/blog/what-a-haskell-study-group-is-not/)
* [Hakyll](https://jaspervdj.be/hakyll/)
* [dataHaskell](http://www.datahaskell.org/)
* [Desugaring Haskell](http://www.haskellforall.com/2014/10/how-to-desugar-haskell-code.html)
* [Understanding basic error messages](http://ics.p.lodz.pl/~stolarek/_media/pl:research:stolarek_understanding_basic_haskell_error_messages.pdf)
* [Specific topics in bitemyapp/learnhaskell](https://github.com/bitemyapp/learnhaskell/blob/master/specific_topics.md)
* [Adapted Agda style guide](https://github.com/andreasabel/haskell-style-guide/blob/master/haskell-style.md)

## Research
* [Safe Haskell](https://www.microsoft.com/en-us/research/wp-content/uploads/2012/01/safe-haskell.pdf?from=https%3A%2F%2Fresearch.microsoft.com%2Fen-us%2Fum%2Fpeople%2Fsimonpj%2Fpapers%2Fsafe-haskell%2Fsafe-haskell.pdf)
* [Practical Probabilistic Programming with Monads](http://mlg.eng.cam.ac.uk/pub/pdf/SciGhaGor15.pdf)

