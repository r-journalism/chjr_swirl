# Some homework before USC's Center for Health Journalism Data Fellowship workshops

Before you join us at R, you need to install the correct software and learn a few new programming concepts. Follow these steps to run these exercises and you'll be well-prepared to hit the ground running at our in-person sessions.

## Step 1: Get R

Install R by downloading and installing it from [this website](https://cran.rstudio.com/). If you already have R, go ahead and download the latest version and install it.

For help installing R, check out one of the following videos (courtesy of Roger Peng at Johns Hopkins Biostatistics):

* [Installing R on Windows](http://youtu.be/mfGFv-iB724)
* [Installing R on Mac](http://youtu.be/Icawuhf0Yqo)

## Step 2: Get RStudio

AFTER you install R, then you can install RStudio, which will make your experience with R much more enjoyable.

If you need to install RStudio, you can do so [here](http://www.rstudio.com/products/rstudio/download/). Select the appropriate installer for your operating system. If you had it installed prior to now, go ahead and do it again to make sure you have the latest version.

## Step 3: Install swirl

You're going to do some introductory exercises to get acquainted with how R works. Swirl is a cool package that loads these custom lessons.

Open RStudio and type the following into the console (the bottom left box with the `>` line):

```
install.packages("swirl")
```

Note that the > symbol at the beginning of the line is R's prompt for you type something into the console. We include it here so you know that this command is to be typed into the console and not elsewhere. The part you type begins after >.

## Step 4: Install the CHJR pre class materials

After you've done step 3, run these lines in the console:

```
library(swirl)
install_course_github("r-journalism", "chjr_swirl")
```


## Step 4: Start swirl

This is the only step that you will repeat every time you want to run swirl. First, you will load the package using the library() function. Then you will call the function that starts the magic! Type the following, pressing Enter after each line:

```
library("swirl")
swirl()
```

## Step 5: Use swirl

Enter your name and run the exercises from `chjr swirl`!

Please run through these exercises before we meet on October 7:

1. Basic Building Blocks
2. Sequences of Numbers
3. Vectors
4. Looking atData
5. Logic  

There are 10 other lessons and you are totally welcome to go over that if you're curious and have the free time! But please prioritize the first four.


## Miscellanious commands if you need them

* Install the `swirl` package:
```
install.packages("swirl")
```

* Install the `chjr_swirl` lessons:
```
library(swirl) # load the swirl package
install_course_github("r-journalism", "chjr_swirl")
```

* Start a `chjr_swirl` lesson (after loading the `swirl` package):
```
swirl()
```

* Uninstall the `chjr_swirl` lessons (after loading the `swirl` package):
```
uninstall_course("chjr_swirl")
```

* Update the `chjr_swirl` lessons (after loading the `swirl` package):  
```
uninstall_course("chjr_swirl") # uninstall the course
install_course_github("r-journalism", "chjr_swirl") # reinstall the course
```