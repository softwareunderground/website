+++
description = "Manage subsurface well data"
title = "Welly"
date = "2019-04-10T16:43:08+01:00"
draft = false
weight = 200
bref="Welly is a family of classes to facilitate the loading, processing, and analysis of subsurface wells and well data, such as striplogs, formation tops, well log curves, and synthetic seismograms."
toc = false
script = 'animation'
repo = ""
website = ""
+++

<h3 class="section-head">Description</h3>

<div class="is-col">
  {{< figure src="../../images/welly.png" alt="Welly" width="100%"
    caption="The typography scale helps to build a balance between the size of headings and text elements">}}
</div>

<div id="action-buttons">
  <button class="button is-secondary" data-kube="toggle" data-target="#box">Show the code</button>
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
