# Zork

## Note: This is an advanced problem suitable for pairs, groups or talented individual students.

Zork was an early interactive computer game. It was initially released in 1977.

According to Wikipedia:

> Zork is set in "the ruins of an ancient empire lying far underground". The player is a nameless adventurer "who is venturing into this dangerous land in search of wealth and adventure". The goal is to return from exploring the "Great Underground Empire" \(GUE, for short\) alive and with all treasures needed to complete each adventure,\[6\] ultimately inheriting the title of Dungeon Master.

We're not going to do all that. But in the spirit of Zork \(and adventure\) write an application that asks people what direction they wish to travel in. Once they tell you the direction, move them to the next room and tell them what is in it and what direction the other exits are.

Your setting will be a seven room haunted house. Good luck!

<table>
  <thead>
    <tr>
      <th style="text-align:left"></th>
      <th style="text-align:left">room</th>
      <th style="text-align:left">contains</th>
      <th style="text-align:left">doors to (direction &amp; room #)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">#1</td>
      <td style="text-align:left">foyer</td>
      <td style="text-align:left">dead scorpion</td>
      <td style="text-align:left">room n2</td>
    </tr>
    <tr>
      <td style="text-align:left">#2</td>
      <td style="text-align:left">front room</td>
      <td style="text-align:left">piano</td>
      <td style="text-align:left">rooms s1,w3, e4</td>
    </tr>
    <tr>
      <td style="text-align:left">#3</td>
      <td style="text-align:left">library</td>
      <td style="text-align:left">spiders</td>
      <td style="text-align:left">rooms e2 &amp; n5</td>
    </tr>
    <tr>
      <td style="text-align:left">#4</td>
      <td style="text-align:left">kitchen</td>
      <td style="text-align:left">bats</td>
      <td style="text-align:left">rooms w2 &amp; n7</td>
    </tr>
    <tr>
      <td style="text-align:left">#5</td>
      <td style="text-align:left">dining room</td>
      <td style="text-align:left">
        <p>dust</p>
        <p>empty box</p>
      </td>
      <td style="text-align:left">room s3</td>
    </tr>
    <tr>
      <td style="text-align:left">#6</td>
      <td style="text-align:left">vault</td>
      <td style="text-align:left">3 walking skeletons</td>
      <td style="text-align:left">room e7</td>
    </tr>
    <tr>
      <td style="text-align:left">#7</td>
      <td style="text-align:left">parlor</td>
      <td style="text-align:left">treasure chest</td>
      <td style="text-align:left">rooms w6, s4</td>
    </tr>
  </tbody>
</table>Here's what your version of Zork will look like at the console:

```text
You are standing in the front room of an old house.
You see a dead scorpion.
You can (1)exit to the east, (2) exit to the west.
1

You are standing in a library.
You see spiders.
You can (1) exit to the north, (2) exit to the east.
```

