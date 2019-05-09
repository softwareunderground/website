+++
title = "Welly"
description = "Manage subsurface well data"
date = "2019-04-10T16:43:08+01:00"
weight = 20
draft = false
bref="Welly is a family of classes to facilitate the loading, processing, and analysis of subsurface wells and well data, such as striplogs, formation tops, well log curves, and synthetic seismograms."
toc = false
website = "https://welly.readthedocs.io/en/latest/"
repo = "https://github.com/agile-geoscience/welly"
+++

<div class="is-width-small is-center">
  {{< figure src="../../images/welly.png" alt="Welly" width="100%"
    caption="The typography scale helps to build a balance between the size of headings and text elements">}}
</div>


<div id="action-buttons">
  <button class="button" data-kube="toggle" data-target="#box">Reproduce the image</button>
  <a class="button outline big" href="{{< param website >}}">Website</a>
  <a class="button outline big" href="{{< param repo >}}">Source code</a>
</div>
<div id="box" class="is-hidden">
  {{< highlight py3 "linenos=table,hl_lines=8 15-17,linenostart=2">}}
  import random

  guesses_made = 0
  name = raw_input('Hello! What is your name?\n')
  number = random.randint(1, 20)
  print 'Well, {0}, I am thinking of a number between 1 and 20.'.format(name)
  while guesses_made < 6:
      guess = int(raw_input('Take a guess: '))
      guesses_made += 1
      if guess < number:
          print 'Your guess is too low.'
      if guess > number:
          print 'Your guess is too high.'
      if guess == number:
          break
  if guess == number:
      print 'Good job, {0}! You guessed my number in {1} guesses!'.format(name, guesses_made)
  else:
      print 'Nope. The number I was thinking of was {0}'.format(number)
  {{< /highlight >}}
</div>
