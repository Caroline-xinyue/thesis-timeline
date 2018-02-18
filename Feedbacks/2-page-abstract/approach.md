On Feb 17, 2018, at 1:40 AM, Xinyue Zhang <
 
On Feb 17, 2018, at 1:40 AM, Xinyue Zhang <xzhang@brynmawr.edu> wrote:

    - Proof Correctness (Soundness): what one language proved but indeed is logically invalid

?? Do you expect this is possible? This would be terrible if you can find a soundness bug.

3. Termination Checking:
    - Check program termination at run time in Haskell

I've talked about "termination checking at run time" in our sessions, but I've really meant this as a joke. A "runtime termination check" is really just running an algorithm and waiting until either it terminates or you get bored.

So, it's hard to compare termination checking, because one language (F*) has it and the other (Haskell) doesn't. Instead, it's better to compare how the two languages deal with potentially divergent computations: Haskell treats them identically to other computations, while F* puts them in Div. What does this choice mean for the expressiveness of the languages? Does this mean that you can prove something in one and not the other? What does this mean for our understanding of what a "proof" means in the two languages?

V.S. termination checking at compile time through a lattice of monadic effects using Hoare Logic in F*

Whoa! A lot of terminology there. F* does have (a) termination checking, (b) a lattice of monadic effects, and (c) support for Hoare logic -- but I don't see how you're trying to connect them in this sentence (and, I suspect, neither do you).



- Library/documentation supports: Is this a way to talk about Hackage for Haskell vs. <<null>> for F*? I suppose it is. But then that's not about language design.

[Indeed I want to talk about Hackage/Hoogle and all the threads supporting Haskell. It's just a general language support that doesn't worth making a whole new metric for, but I am not quite sure how to expand the first metric to contain this as a sub-area of interest.]

I think, in the end, hewing too closely to these metrics isn't going to serve you well -- not everything you want to say is going to fit neatly into one of these bins. Yes, having clearly defined comparisons you wants to draw and tools you will use to draw them is very useful, but some ideas will just fall outside.


- Adaptability of proofs: What do you mean by this? I can think of several meanings, but I'm not sure which you're thinking of. Could you expand?

[Originally I was thinking about the complexity of proof writing. For example, in the QuickSort case, F*'s intrinsic proof using refinement types in addition to some unavoidable lemma-proofs helps make the verification in general much easier.]

OK. That makes sense. But that's not "adaptability". What you're really talking about here is how easy the proofs are to write.


- Effectiveness of proofs: I'm not sure what this is. Are you worried about whether or not the proofs are sound? Are you worried about what can be proved? If it's the latter, then this is the same as type system expressiveness.

[Yes, soundness is what I mean.]

I still want to understand this better. What soundness worries do you have?


- Quantified success rates: Rates of what, precisely? To be able to quantify a success rate, you need a benchmark suite. To my knowledge, none exists. We could make a benchmark suite, but then it is trivial to cook the numbers.

[I wasn't quite sure on the termination part, so I was thinking of potentially doing a quantified analysis. But now I believe I should focus more theoretically on the F* effect system and its termination checking against Haskell approach to verify program termination at run time]

Quantified analysis is great -- but of what, precisely? I don't know. The rest of this statement then goes back to my comments about about termination checking.

So: if you want to have a clearly delineated list of aspects to compare and metrics to compare them by, I think you still have more work to do. It's not really tight enough yet for me to be able to understand your intent.

Thanks,
Richard

 


Thank you again for your help!

Sincerely,
Xinyue
From: Richard Eisenberg <rae@cs.brynmawr.edu>
Sent: Friday, February 16, 2018 2:18:21 PM
To: Xinyue Zhang
Subject: Re: Regarding the 2-page thesis abstract feedback
 
Hi Xinyue,

It's not the wording -- it's your choice of metrics.

- Syntactic verbosity: OK. This one is fairly apparent, but not really all that interesting.
- Type system expressiveness: This is a big one! In some sense, this covers all the comparisons that you would be doing. By putting this under "language design", I'm not really sure what it means.
- Library/documentation supports: Is this a way to talk about Hackage for Haskell vs. <<null>> for F*? I suppose it is. But then that's not about language design.
- Adaptability of proofs: What do you mean by this? I can think of several meanings, but I'm not sure which you're thinking of. Could you expand?
- Effectiveness of proofs: I'm not sure what this is. Are you worried about whether or not the proofs are sound? Are you worried about what can be proved? If it's the latter, then this is the same as type system expressiveness.
- Quantified success rates: Rates of what, precisely? To be able to quantify a success rate, you need a benchmark suite. To my knowledge, none exists. We could make a benchmark suite, but then it is trivial to cook the numbers.

I do think it's good to nail all this down ahead of time!
Richard

On Feb 15, 2018, at 5:37 PM, Xinyue Zhang <xzhang@brynmawr.edu> wrote:

Hi Richard,

In my abstract, I presented my approaches for comparing Dependent Haskell and F* on the three aspects. Specifically, I wrote:

"We will structure the comparison mainly focusing on three aspects: language design measured from syntactic verbosity and type system expressiveness, and library/documentation supports; verification techniques determined through the adaptability and effectiveness of proofs; and finally termination checking evaluated using quantified success rates as metric."

You commented that you don't understand these aspects, but it seems that my peers and Dianna understand my methodologies. I am wondering if it's the awkward phrasing/wording or the actual content that confuses you. I am planning to rewrite my approach accordingly.

Thanks in advance!

Sincerely,
Xinyue
