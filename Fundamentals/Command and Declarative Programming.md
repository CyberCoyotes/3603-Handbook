# COMMAND BASED
##
There are two approaches to making an FRC robot: **Imperative**, and **Command-Based**, of which we use the latter.
<br/>

# Imperative
Imperative is like designing a linear list of orders for the robot to follow.
It's hard to properly communicate the differences between the two philopsophies in a tl;dr format, but the cliff notes are that Imperative is what most inexperienced people would default to. While it's easier in the very short term, the drawbacks are too large to be viable; added maintenience, dependency, and ambiguity in control flow are all reasons to avoid imperative.


# Command Based (and declarative)
Command based is like designing a set of rules for the robot to follow.
A quick distinction is in order:
"Command-Based" refers to the way robot properties and actions are broken into **subsystems** and **commands**, with a large arsenal of classes and functions to help with the subsystems and commands. "Declarative" programming is the ~~programming Paradigm~~ more sustainable, effective method of programming that goes with command-based like PB+J. For this reason, they will often be grouped together as simply "Command-Based" (occasionally, "sane, functional human being code") 

##
# A quick table, summing up the uses
<table>
<thead>
  <tr>
    <th>Issue</th>
    <th>Imperative</th>
    <th>Command-Based + Declarative</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Quick prototyping</td>
    <td>Good; makes it easy to prototype simple code</td>
    <td>Not needed; thinking about code structure for simple tests and whatnot isn't needed,</td>
  </tr>
  <tr>
    <td>dependence</td>
    <td>nightmarish; like soldering a lamp to a socket</td>
    <td>Non-existent (if you're smart) due to much more modular design</td>
  </tr>
  <tr>
    <td>Reading and comprehension</td>
    <td>Fine for short snippets of code, <br>but complex systems and developers will suffer greatly from the inherent <br>lack of clarity</td>
    <td>Easier to separate each function call and class into individual parts, <br>and debugging can be made much easier (if you're smart)</td>
  </tr>
  <tr>
    <td>Issuing Robot Orders</td>
    <td>Calling robot methods directly; easy to understand for a whole 5 seconds,<br>dependencies will FESTER</td>
    <td>Robot properties and actions are neatly fit into subsystems and commands, <br>allowing for greater control and mental ease</td>
  </tr>
  <tr>
    <td>reaction of pretentious team 1XX member</td>
    <td>dude what is this youre disgusting</td>
    <td>this is so good marry me</td>
  </tr>
</tbody>
</table>

###

If you yet hunger for perfection beyond Declarative, check out the SOLID principles, one of the most popular set of guidelines for clean code out there. I would recommend watching Tim Corey's videos on the priciples. They're boring as *redacted*, but they are presented carefully enough to actually teach. Another caveat is that he uses C#. Even though he uses a different language, the priciples still apply in Java. Also, C# and Java are very similar in basic syntax, with differences you don't need to worry about yet. 