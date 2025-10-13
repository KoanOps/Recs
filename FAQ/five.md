5 Important ideas in Machine Learning

1. Conditional distributions: It's a deceptively simple idea:
Suppose you want to estimate a distribution, P[X], and it's incredibly difficult to write down an exact formula for it. Ok, you can always condition on ANYTHING Z, and say that P[X | Z] is easy, because you have more specific information. 
This is the basis for so called "plug in" estimators. Markov Chain Monte Carlo generalizes this idea. The point is to say, I want to estimate some distribution as the limit of some other conditional distribution. 
In math and physics this technique shows up a lot: the Hamiltonian of some system is usually way easier if you think of it as a potential of mean force of a larger system by adding in Lagrange multipliers
That's a fancy way to say, I can (often) think of a solution in a larger space with more symmetries that makes the optimization problem easier.

Turn a hard estimation into an optimization problem, and then work to make the rate of convergence of that optimization problem fast enough to be useful. MCMC methods basically embed your desired distribution as a limit of a process embedded in a larger space.
For example, the so-called Metropolis-Hastings algorithm embeds the problem into a proposal conditional distribution

Like with Fourier transformation in signal processing. No that's an issue of rotating the problem into a more convenient basis.

Nearly every sophisticated ML model you see is just embedding into a larger space that makes optimization easier. For example you can think of random forests as an axis aligned (Each feature dimension is an axis) conditional estimator of the Bayes optimal estimator.
That's like saying, I want a shitty conditional estimator as a plug in distribution that is a discrete estimator for how far are different datapoints

My point in all this is that you should always try to find a place to stand to look at a problem where it becomes simpler

Because often a naive but useful algorithm will emerge. And that's why Bayesian methods are alluring - they weaponize conditional distributions

Is there a case where reducing the space would help the optimization as well?
When two dimensions are too similar
When a dimension is insignificant to a problem you are trying to solve
Simplifying the model sacrificing accuracy for optimization speed
Really think carefully about the idea of the conditional distribution and think about the Glivenko-Cantelli theorem. https://en.m.wikipedia.org/wiki/Glivenko%E2%80%93Cantelli_theorem (Really really think simply and deeply)

I built a black literman model with views from random forest, correlation matrix was replaced by inverse wishart distribution which is the prior and historical data which I downloaded from Yahoo finance. 
Also the model was under non linear constraints (skewness, kurtosis) . I tested it on 12 stocks. It worked on 7. By worked I mean the prediction was closer to the real value. Correlation matrices come up pretty strongly in stochastic local volatility and building vol surfaces in options. 
Quantitative marketing is mostly causal inference writ large no?  There are various approaches to marketing with ML and probabilistic models. Market research, using focus groups as priors, etc. 
But human sentiment is as fluid as language, perhaps more so. And marketing to a B2C crowd is as fickle as a breaking a ornery horse. "Own" becomes "slay" and "slay" becomes "eat". 
Just like we see convulsions in language, we do in marketing. Supreme is cool now, could be passe tomorrow. Revolve goes around revolving around the world, until it doesn't. 
So forth and so on. Dealing with industry vertices and the shifting tastes of consumers is both a quantitative and qualitative thing.
And you have to understand people. This is always forgotten. I mean on a basic level. 
And it matters from segment to segment. Some are faster to change, some are slower, some are cyclical with tweaks (fashion, for instance). 
And then there is direction. The community didn't want an iPad. But it adopted them. That comes from Jobs, for as much of a bastard as he was, understanding people in a very intrinsic way.
You either get people or you don't. It's a talent. The best do. The rest build models and try to. Years of experience as a consultant. You see it all over, executives who fundamentally don't understand people, in consumer facing roles. 
People are weird and emotional. Consumers, I mean. There are also cyclical trends in fashion, this is well known. What's old is new again, and those can be predicted with some regularity. How they are predicted is really, really non-PC, in some cases however.
(understand people like social skills/artistic/peoples feelings way, But mainly I'm meaning they understand how people think. They sort of "get" people in a way that allows them to see what can be cool. Trend dictation, not anticipation.)
It's a nightmare to fix, because you cannot teach understanding people. Phrasing matters. "invest" is an "expense term" "save" is a, well, savings term. Which is something that you only understand at the very big frames of reference.
Sales is about building a relationship and selling a product. Marketing is about building a brand.

Once you understand the five or so major tricks in machine learning you can do anything
