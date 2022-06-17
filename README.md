# PHP-Debugging

a Becode project

Learning objectives

understanding the root of bug fixing
know what print_r, var_dump, die, echo, exit, break do
know what to do the next time you're stuck
give yourself the solver's mentality, a problem is just an opportunity to learn!

The Mission

Debugging is the pinpoint to being a master in any coding language.
Everyone gets errors, but the best programmers never let it stop them and they find a way to fix it every time! I scoured the internet for a debugging guide, that I felt like I could get behind and here it is: The guide

This is what I feel like doing when coding PHP that doesn't mean that this should be your way. Discover, look up, research whatever ways work for you to debug you code!

I very much encourage you to use xDebug as much as possible!

Must-have features

Open up the junior.php.broken file, read the comments, fix the code blocks as requested in the comments and put the final file expert.php in the repository folder as requested.

You will change this junior code in expert code!

// === Exercise 1 ===
// Below we're defining a function, but it doesn't work when we run it.
// Look at the error you get, read it and it should tell you the issue...,
// sometimes, even your IDE can tell you what's wrong
echo "Exercise 1 starts here:";

function new_exercise() {
$block = "<br/><hr/><br/><br/>Exercise $x starts here:<br/>";
echo $block;

}

Solution: I ran the new_exercise function and put a breakpoint on it before using "the listen for Xdebug" function. The page on my local host then informed me of an undefined variable $x on line 5. I gave the variable $x a value which fixed this error.

new_exercise(2);
// === Exercise 2 ===
// Below we create a week array with all days of the week.
// We then try to print the first day which is monday, execute the code and see what happens.

$week = ["monday", "tuesday", "wednesday", "thursday", "friday", "saturday", "sunday"];
$monday = $week[1];

echo $monday;

Solution: Variable $monday is set to index 1 of the array so it will give tuesday instead of monday. We will set it to index 0 to fix this exercise.
