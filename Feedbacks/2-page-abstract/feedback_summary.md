- [ ] Definition of Haskell and F* (F* is not a version of Haskell)
  - [ ] Haskell (TT + Dependent Types) Inspired by Martin Lof Type Theory(can only see differences in data; functions and case[bool maybe, either, list(finite set of structures){make decisions on the types introduced by `data`}])[Type Families(differentiating differences between types as int and bool) etc]
  - [ ] F* (SMT + Dependent Types + Refinement Types)
- [ ] Definition and examples of Functional Programming terms
  - [ ] Type Safety
  - [ ] Verification-based languages
  - [ ] General-purposed languages (programming effects, error, IO, stateful programming ...)
  - [ ] Dependent Types
  - [ ] Refinement Types
  - [ ] Type Theory
  - [ ] Satisfiability Modulo Theory
  - [ ] GADT
  - [ ] Type Families
- [ ] Purpose and Motivation
  - [ ] Why we want to compare? What to achieve? 
  {
  languages[verfication approaches], provide next step to the community
  long time dependently typed languages: since coq(longest 80s), adga, idris
  functional languages: Haskell, ML, Racket
  motivation for the current space: lightweight, practically-oriented verified programming languages -- DH, LH, F*, Idris[these 4 are new but also functional], maybe Ada(may not be functional) [young field, sharing]
  Idris is more understood based on Martin Lof Type Theory, DH, F* non-termination, extensions to ML type theory to be more applicable [DH: Type family, typeintype; F*: effect system]
  DH, LH, F* compared exploratively in my poster
  
  put resources into the right method. Is it worth it to try the other approaches
  }
  - [ ] What potential collaborations(Haskell and F* [termination])? How does it help Programming Languages in general?
  - [ ] Why we want fully-fledged dependently-typed haskell(explain what does more precise expressions of program specifications mean?)
- [ ] Detail but not everything about the results
- [ ] Relationship with the previous work (how the explorative work leads to the specific/focused thesis)
- [ ] Details (Clarification)
  - [ ] Elaborate how DH and F* are different (how they categorize programmming effects differently) [define effects]
  - [ ] Background help readers follow {audience}
  - [ ] TT and SMT are not in competition (wouldn't call them mainstream)
    {TT structures for the proof building blocks; SMT powers the actual proof}
  - [ ] More Examples

- [ ] Check contents:
  - [ ] TT-based Dependent Haskell and SMT-based dependent-and-refinement-typed F* each represents a unique and effective program verification technique. They are similar in that they both aim towards a verification-based yet general-purposed programming language, but they are noticeably different in their unique approaches to categorize programming effects.
  - [ ] Specify the collaborations
