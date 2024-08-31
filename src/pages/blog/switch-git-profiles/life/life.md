## Day 1 - 8/21/2024
Until I find a way where I can link different chunks of a really long journal where I document different parts of my life I'll settle with manually writing my process and linking videos using markdown and mdx

I probably should write this so I don't forget
```
Make sure to create some way to highlight parts of your journal and assign them to different blogs depending on if it talked about or related with the project
Some sort of documentary in a documentary.
Figure out a way to make unhighlighted chunks in the journal private and make even the highlighted chunk private if it needs to be

Also create a UI for that or add that to your markdown flavor or both?
```

Alright back to life
I'm thinking of creating a bash script I could run that replaces the default ssh and configs based on the user

Something like
```bash
$ custom-program -list
```
would list the users

```bash
$ custom-program switch user
```
would switch to that specific user

```bash
$ custom-program generate ssh user
```
would generate the ssh for a user so you just use that instead when setting up

```bash
$ custom-program add-config user.name username
```
For adding custom configs

Also figure out how the hell astro knows which syntax highlighting to use, that's really cool

In the meantime you got to trust me on the dates lol

## Day 2 - 8/23/2024
I just sorted myself out with my calendar and have a strict schedule I'll be following.

For now I'll be focusing on scripting and shell commands because of this project and a class I am taking.

I should start working on the script tomorrow for switching git profiles.

## Day 3 8/26/2024
I got my vm set up, dealt with something's on my end. And now there's actual progress.

I'm currently working on a way to create a class in python that installs a libary for the generation of the public/private key with ssh

List of things to do
- Create a way to know which user is currently active
- Create a way to switch git config files (at ~/.gitconfig)
- Create a way to generate public and private ssh keys with passphrase support
- Create a way to update the .ssh/config file anytime a user changes
- Create a way to store the current config file of a user before switching over to the next

Later I'll deal with logic for switching the gitconfig files at `/etc/gitconfig` and `.git/config`


This is me from much later in the day

*Side note: maybe make a python program that records all commands/buttons pressed in a blender session, that way you could work alongside professionals and see what they did at each point while having a video that shows what that did, like a timestamp*

Alright so I was able to create a command that runs the ssh-keygen command and I've figured out a rough and somewhat strict workflow on how I want the utility to work. I should be done with the first version tomorrow and then focus more on making my website public and adding a regression testing framework to it before finally making it look good.

## Day 4 8/27/2024
I am done with a rudimentary system for switching users. Going forward I'll work on failsafes to make sure my accounts don't bleed into each other but with enough caution this should be good enough to manage my identity efficiently and start my website. - TheCist

# Day 5 8/29/2024
Had a busy day yesterday, school stuffs and internship approvals, so much bureaucracy after saying yes. It's kind of frustrating but I never liked paperwork so that's expected

That aside I've gotten the user manager up and running! And it's had it's first test dummy(me)! Chatgpt came up with a good name, gitSwitch. I like it so I'll be using it as the name of the program.

I'll be working on moving the current website code over and start with the regression tester