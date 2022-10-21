So say you have installed v2 and now you want to set up VS Code for it

That used to be kinda complicated, but now there is a nice extension you can install

Search up "Autohotkey v2 language support" and install this extension

Well, thanks for watching and...

Nah, just kidding

Technically, you're done, but I want to actually show you what you're gonna get

That way you can use the tools provided to their full potential

First of all, make sure your v2 folder isn't renamed from what it was after the installation

If you renamed it already, rename it back to the default shown on the screen

Now go back to some v2 script

Ctrl shift p and search for "search language mode"

Configure for .ahk, autohotkey2

You might have noticed this button on the bottom left

You can use it to choose a version used to run your ahk scripts from vs code

One **HUGE** disclaimer: do **NOT** choose the UIA versions, for whatever reason, they fuck up the extension to the point that you can't even change it back and 
everything breaks

Goddammit Axle you should've said so sooner!

Don't worry, I have a solution for that

Search up settings json

If you just have a folder open, choose folder settings

If you set up a workspace, choose workspace settings

You'll end up in this json file that has the interpreter as a setting

Go ahead and manually change the exe to the one without UIA

Reload Vs Code, and everything should be fixed

Now, you don't actually have to click that button to choose your interpreter

There's a command you can look up to reach the same effect

So, if you want to, you can hide the button by right clicking the gutter and pressing hide

Now, there are a few really useful commands I recommend you use

By typing in "ahk2" in your command palette, you'll see all the commands from the extension

Definitely check all of them out, but I will go over the two most useful ones

Let's first write some example code and set some breakpoints

Make sure **this** extension is also installed

And now, we can debug our v2 scripts

Notice how I didn't need to set anything up?

Yeah, we don't actually need to make a launch json or anything of that nature, just use the command

On the right, you'll see your variables

Nothing appeared in the local section because my variable is actually global, let's change that

Now the age variable appeared in the local section as it should be

After we go over the line, the variable is initialized

One cool thing I haven't seen before is that we get the time it took to execute the line, so you can more easily see how well your code stands in terms of performance

When you debug, you can use the outputdebug command and it will actually appear in the debug console

By the way, your debug console is likely to be in the bottom panel by default

You can move it to where *I* have it if you want to, vs code is very customizable like that

All right, we went over the debug command, but you don't have to debug to just run a script, there's a command for that too

Search for "run script"

And the extension will run the active script with the interpreter we chose earlier

The output panel will pop up that'll say the script ran

And when that script exitapps, will say so with the exitcode and time the script was running for

You'd think outputdebug would work with this panel too, but unfortunately it only works in the *debug* console

Alright, lemme teach you how to color your code however you want

Search for tokens and press enter

You'll see this menu

What you need to look for is the topmost line in textmate scopes

Select and copy it, then go to your settings.json

First, editor token color customisations

Then, textMateRules

And here you'll color your code from now on

Let's create an object, it's going to have the scope of what we just copied

Now we create the settings object with two properties

Foreground is where you set the actual color

It accepts hex values for that

And don't worry if you don't know how to get a hex color, because in the actual settings, you'll be able to choose it in this gui

Now for the font style, leave it an empty string if you just want the normal font

But there's also bold, italic, strikethrough and underline

Now say you want to paint some code class the same color

And you don't want to create an object for every code class

Make your scopes an array

And go on, adding more and more classes

***Unfortunately, the rest of the transcript was lost. Won't happen in newer videos***
