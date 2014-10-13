#GHC Linux Kernal Hacking
**The Kernal Hacking Cycle**
	- find a contribution to make
		- read stored communications
		- gain experience
		- ask questions : become part of the collaborative community
	- code your contribution
	- send it in
	- gather feedback
		- testing results
		- mentoring and guidance
		- discussion of strategies
		- general suggestions
	- incorporate changes
		- use feedback to improve
	- repeat.
**Communications**
	- mailing lists
		- LKML (Linux Kernel Mailing List)
	- private email
	- conferences 
	- linux weekly news
	- IRC
**Coding your changes**
	**Plan** 
		- trace existing paths of execution
		- don't cowboy code
		- find examples similar to your goal
		- learn which lines are relevant
		- your friends are 'grep' and 'lrx ident'
	**code**
		- language is c
		- follow kernel coding style
		- gain skill with your editor 
	**compile & run**
		- this involves installation and rebooting
		- use a virtual or dedicated machine (KVM using that as coding env)
		- maintain a known working and a test kernel
	**test & debug**
		- printk()
		- find messages in /var/log/kern.log
		- create testing scenarios 
**Delivering your patch**
	**git commit strat**
		- make small incremental changes
		- make changes in logical order
		- each change should be encapsulated (bisceptable: you can split the code at any point and be clear what came before and after that point)
		- be prepared to alter previous commits
		- be prepared for upstream changes as you update your sources
	**git branching strat**
		- keep master branch unmodified
		- create a working branch
		- use throwaway branch to squash commits (tiny commits -> large commit)
		- if this doesn't work, find a way. 
	**composing the commit message**
		- work as hard on this as you do on coding
		- why you made changes, what the changes are. This is all documentation
		- read existing examples
		- be concise, yet thorough
		- use imperative language
	**the patch**
		- run checkpatch.pl on the files you change (will find any nitpicky coding style issues)
		- generate patch with a git command
		- cc everyone involved with the code.
		- send using plain text mail
			- because email formatting will break your code
			- team members will apply your patch as is
			- commit message will become subject line and content
			- use a specific mail client such as mutt
