---
published: false
layout: post
title: Gus' Paradox
date: 'Sun, 19 Sep 2021 02:18:53 -0400'
category: meta
tags: theory
mathjax: true
---

When you work full-time every day it can be difficult to write a blog. This is specially clear when you have a job that uses a lot of your intellectual energy or is physically demanding. In this post I'm trying to psyche myself, or rather, trick my mind, that daily posts are simple; but first I want to define the blog post's value.

The other day I was reading a great, and short, post titled [_"Write 5x more but write 5x less"_][1] where the author states:

> There are 2 things I have come to believe about writing:
>   1. The average person should write 5x more things than they do.
>   2. The average written thing should be 5x shorter than it is.
>
<cite>&mdash; [Write 5x more but write 5x less. (2020, October 2). Call me Critter. Retrieved 23:45, September 20, 2021](https://critter.blog/2020/10/02/write-5x-more-but-write-5x-less/)</cite>

Let's call it, _Critter's Rule_.

The first point makes sense to me and I can agree to most of his reasons why we should write more often. Anything that helps you think should be done greater and often. I would like to add a few more reasons:

- Because writing helps your career; showing what you know.
- Because writing can help you make new friends; sharing what you know or don't know.
- Because writing makes you a better person.

Now, the second statement in _Critter's Rule_, about writing shorter, is a bit vague to me.

I agree that we live in busy and congested times, and that we don't have or want the luxury of waiting. That the reader's [average attention span has reduced][3] from 12 seconds in 2000, to just eight in 2015 (I bet it's 3 secs now in 2021). Not to mention that adult ADHD [appears to be rising][4].

The reason why his second point confuses me is that somehow he claims that it can be explained with the **80-20 rule**, also know as the [Pareto principle][2]:

> The Pareto principle states that for many outcomes, roughly 80% of consequences come from 20% of causes (the “vital few”).
>

In other words, that 80% of the results come from 20% of the effort.

But if you examine the definition of the _Pareto principle_, you can notice that it has to do with outcomes, results. And if we apply it to writing it would mean that _80% of your blog posts will be crap, and only 20% will be good_. Since the result of a blog post is the value it returns to the reader, I can see why "PP" would seem to fit.

I would like to offer my own theory, which I call **Gus' Paradox** or the _Law of Dimished Interest (LDI)_:

## Law of Diminished Interest (Gus' Paradox)

> The value of a blog post dimnishes proportional to its effort and age.
>

Represented with the equation:

$$
  V_t = Q(\omega)
$$

Where \\( V_t \\) is the value of a blog post at some constant time \\( t \\), and \\( Q(\omega) \\) is the quality as a function of the number of words.

There's a lot compacted in there, let me explain.

### Explanation

According to _Critter's Rule_, a blog **author** gets enough value from writing often. There is [plenty][5] of [literature][6] that [supports][7] [this][8]. But if we focus on the **reader** 👀, then it becomes clear that the value is what they can get from the post.

Unfortunately, the post's value diminishes with time as it may become irrevelant or obsolete. Also, the reader's interest may diminish the longer the author mulls the post's points (like I'm doing now).

Books have an intrisic literary value and quantified length. Even if the content of a book is obsolete it may retain its value as a reference. We also assume a book has gone through several rounds of validation by its authors and editors.

In contrast, blog posts are random events of unqualified value and length. They can be long or short, accurate or opinionated, real or fake.

Let's geek this out!

### LDI as a value function

When the number of words in a blog post \\(\omega \ne 0\\), we define a [value function][9] as a relationship between value and quality:

$$
  V_t = Q(\omega)
$$

Where \\( V_t \\) is the value at specific time \\( t \gt 0 \\) and \\( Q(\omega) \\) represents the effort by the reader and its interest, known as post quality.

We can rewrite \\( Q(\omega) \\) as a _Hamiltonian function_ maxima:

$$
  V_t = \max \int_{t_0}^{t_1} W(\tau,\omega) + \lambda \cdot I(t_1)
$$

Where \\( W(\tau,\omega) \\) is the reader's effort at any time, and \\( I(t_1) \\) is the interest at the latest time.

In conclusion, I claim that the value of a blog post diminishes proportional to the work required to read it and the age when it was posted.

### Conjecture 1: WTF Conundrum

For \\( \omega \to 0 \\) and \\( t \to \infty \\) we notice that the effort is trivial and we are only left with empty interest:

$$
  \begin{aligned}
  V_\tau = \lambda; \\
  \lambda \approx 0
  \end{aligned}
$$

Therefore reader is left with value expectations that are not met.

### Conjecture 2: Wasted effort (F*** it Principle)

The only quantity we can control in a blog post is the number of words; their worth is trivial because it is highly subjective. And the number of words has a direct effect on the reader's production value, because everyone reads at different levels of efficacy and comprehension.

So we can infer that:

$$
  2 \cdot Q(\omega) > Q(2 \cdot \omega)
$$

Or that two (2) posts are better than a single post that is twice as long. This observation is inline with [diminished returns][10].

### LDI Proof

I will work on proof(s) with more blog posts &mdash; stay tuned.


[1]: https://critter.blog/2020/10/02/write-5x-more-but-write-5x-less/
[2]: https://en.wikipedia.org/wiki/Pareto_principle
[3]: https://www.yahoo.com/lifestyle/you-probably-dont-have-a-long-enough-attention-118972368757.html
[4]: https://www.cnn.com/2019/11/01/health/adult-adhd-rising-study/index.html
[5]: https://medium.com/the-brave-writer/how-writing-changes-your-brain-75c9087f37e7
[6]: https://careerconnections.smeal.psu.edu/blog/2018/06/07/how-strong-writing-skills-benefit-your-career
[7]: https://www.cosmopolitan.com/sex-love/a26658784/journal-love-life-dating/
[8]: https://www.huffpost.com/entry/writing-health-benefits-journal_n_4242456
[9]: https://en.wikipedia.org/wiki/Value_function
[10]: https://en.wikipedia.org/wiki/Diminishing_returns
