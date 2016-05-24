---
layout: post
title:  "A sieve of Eratosthenes in python"
date:   2016-05-24 11:15:13 
categories: programming
---
A while ago, a friend of mine asked me how good I was with programming. I'm not a programmer (yet), but I do manage to write some code every now and then. So he posed me a question, whilst sitting at a bar. "Write a sieve of Eratosthenes, in your favorite language. You have one hour, see how far you get. The upper bound will be 2^20"

At first I had no idea what he meant, but after explaining the algorithm it should be possible to implement. After some additional reading on wikipedia about the [sieve of Eratosthenes][sieve], I set out to program the next morning, whilst enjoying the morning commute. This particular commute would last about 70 minutes, so I had some time to find a seat, and start up my trusty laptop. 

## Finding primes
Finding prime numbers is what a sieve does. And it does so in a very simple way.

+	Generate a list of all numbers from 2 up to the bound, then cross off all multiples of the smallest prime, which is 2, so that would be 4, 6, 8, 10 

+	Then do the same for the first number lager than this prime (which would be 3 in this case) and cross off all multiples: 9, 15, 21 ... note that 6, 12 and 18 were already crossed off the list. 

+	This continues until all values that have not been crossed off, have had their multiples crossed off. 

<em>Note to self: learn how to explain algorithms in a way that people will understand them.</em> 

## The code

This is what I came up with. As you can see, I might be seen as a verbose programmer. I like to add profuse comments to small pieces of code to explain (to myself) what is actually going on.
This helps me understand what I wrote, when I come back to the code, as I do not see code every day.
As an added benefit, you can now enjoy a detailed python implementation, including comments for each step.

{% highlight python %}

import math # For the sqrt function

upperBound = 2**20
print "Please give an upper bound, maximum is %r" % (upperBound)
bound = int(raw_input())

# checking input for upper bound
if bound > upperBound:
	print "Given bound out of range"
	exit(1)

# Initialize array needed
primeArray = (bound+1) * [True]

# The algorithm itself
for i in range (2,int(math.ceil(math.sqrt(float(bound))))):
	if primeArray[i]:
		for j in range (i**2, bound+1, i): # i*i might actually be faster
			primeArray[j] = False

# Print the array
print "Prime numbers in range (2,%i)" % bound
for i in range (2, bound+1):
	if primeArray[i]:
		print i

{% endhighlight %}

[sieve]: https://en.wikipedia.org/wiki/Sieve_of_Eratosthenes

