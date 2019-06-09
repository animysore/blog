---
layout: post
title: Regex Substitution to structure raw data
description: Regex use case - Converting data copy pasted from a PDF into a JSON file
tags:
  - Regex
image:
  feature: "abstract-11.jpg"
comments: true
share: true
published: true
---

## The Challenge:

Regular Expressions ( aka the regex ) are powerful tools for doing string comparison (and substitution!). I was recently building an online practice quiz app - with javascript - and I needed to create a JSON database of the questions and answers. Of course, as my luck would have it, all the questions were on a pdf. There was no way to directly convert this to the format I needed.

The Raw data:

![The raw pdf data](/blog/images/2017-02-02-regex-magic/original.png)

My required format:

{% highlight json %}
    [   
        {
            "question": "this is the question text",
            "options": ["choice1", "choice2", "choice3", "choice4"],
            "answer": 2
        },
    ]
{% endhighlight %}

I had five files in total, with the question count being 440 or so. Typing was out of the question. So I decided to go with Submlime Text's search and replace. Sublime supports regex search and substitution. This entire exercise has been a real eye opener for me.

I hope this post serves as a rough guideline. The chances my exact code will be useful in any other case are very slim. 

### Step 1 : Copy from PDF to a text file

First I copied everything in the pdf to a plaintext file. ctrl+A ctrl+C ctrl+V

Result:

![Result after simple copy paste](/blog/images/2017-02-02-regex-magic/copypaste.png)

There seems to be rough order, with the question and each option being on new line. Questions and options are preceded by a number or an alphabet. Now this is a small snapshot of the file. This format was more or less consistent throughout the file, but with the occassional aberration. I have not included those here for simplicity's sake. And now, to start writing my Regular Expression!

### Step 2 : Target the pattern

I'm still a rookie when it comes to regexes. This is a simple project, but it still took a considerable amount of trial and error, and after much playing on two regex testing sites [Regex 101](https://regex101.com) and [RegExr](http://www.regexr.com/) I finally got the required regular expressions.

{% highlight bash %}

# Since each question is preceded by a number, we can use this to target questions

[0-9]{1,3}\.\ (.*)

# similarly the options have are preceded by the letters A-D
# I actually wrote this 4 times these because I could not get the groups to play along nicely

[A-D]\.\ (.*)\n # x 4 times. sigh
  

{% endhighlight %}

If you aren't sure what these cryptic characters mean, here's an explanation:

![Explanation by Regex 101](/blog/images/2017-02-02-regex-magic/explanation.png)

### Step 3 : Replace!

Now this is where the magic happens. Regex substitution lets you use the matched 'groups' in your substitution. I am going to make use of this feature to generate my structured JSON file.

{% highlight bash %}

# For the question :

\n\t{\n\t\t"question" : "$1"

# For the alphabets : 

\n\t\t"choices" : ["$1", "$2", "$3", "$4"],\n\t\t"correctAnswer": ""\n\t},

{% endhighlight %}

## Putting it together 

Mashing together the individual pieces, to form the final search and replace expressions gives very satisfactory feeling. The expression used for searching is very poorly constructed, and can definitely be improved. I repeated the same term 4 times because I could not get the grouping construct to work.  

{% highlight bash %}

# regex search

[0-9]{1,3}\.\ (.*)\n[A]\.\ (.*)\n[B]\.\ (.*)\n[C]\.\ (.*)\n[D]\.\ (.*)

# regex replace

\n\t{\n\t\t"question" : "$1"\n\t\t"choices" : ["$2", "$3", "$4", "$5"],\n\t\t"correctAnswer": ""\n\t},

{% endhighlight %}

Here's how it looks, in action:

![Gif of final regexes in action](/blog/images/2017-02-02-regex-magic/rec.gif)

And that's the way it's done :neckbeard: