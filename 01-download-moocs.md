# How to Research Almost Anything Part 1: How to Download MOOCS and Youtube Tutorials

by [@timothystiles](https://twitter.com/TimothyStiles)

This is the first part of my tutorial series **How to Research Almost Anything**. This series will teach you: 

1. [How to download tutorials and course material from youtube, edx, and coursera.](01-download-moocs.md)
2. [How to find almost any book with libgen and the gutenburg project.](02-find-almost-any-book.md)
3. [How to access almost any scientific article with sci-hub, unpaywall, and the openaccess button.](03-access-almost-any-scientific-paper.md)


In this first tutorial I'm going to show you how to save youtube tutorials, edx courses, and coursera courses for later just in case they later get taken down or paywalled.


## Installation
First you're going to need to [install pip](https://pip.pypa.io/en/stable/installing/) if you don't already have it on your computer. **This involves the command line**.

Then you're going to use pip to install youtube-dl, coursera-dl, and edx-dl.

```
pip install youtube-dl coursera-dl edx-dl
```

## youtube-dl
Say you have this awesome youtube tutorial or maybe a short video about your [local community biolab](https://vimeo.com/259874563/c2b3c3a57f) on youtube or vimeo that you want to save. Just fire up your command line and run the following:

```
youtube-dl https://vimeo.com/259874563/c2b3c3a57f
```

The video will appear in your current directory which you check by running `pwd`.

`youtube-dl` can download videos from a view other sites besides youtube. If you'd like to learn more check out their [github page](https://github.com/rg3/youtube-dl) or run:

```man youtube-dl```


## edx-dl
Edx is pretty great about making sure that all of their course material is freely available at no cost. They also have great intro classes like [W3c's Front-end Basics Intro](https://www.edx.org/school/w3cx) or [MIT's Intro Bio Class](https://www.edx.org/course/introduction-biology-secret-life-mitx-7-00x-7).

My community lab has a study group that follows along with [MIT's Intro Bio Class](https://www.edx.org/course/introduction-biology-secret-life-mitx-7-00x-7) but the course isn't alway available at certain points of the year and I like use edX courses like reference notes so naturally I thought it'd be good to show everyone how to archive these classes for later.

Try typing the following into your command line or terminal:
```
edx-dl https://courses.edx.org/courses/course-v1:MITx+7.00x+1T2018b/course/
```


You should get an error asking you for your username and password:

```
edx-dl: error: the following arguments are required: -u/--username
```

edx-dl requires you to use your edx username and password and **already be signed up for the course that you're trying to download.**

```
edx-dl -u user_email_address -p user_password https://courses.edx.org/courses/course-v1:MITx+7.00x+1T2018b/course
```
That should download all lectures onto your computer that you can view anywhere at your leisure. Some notes may come along with the lectures.

## coursera-dl

Coursera has this new thing where you can sign up for a free 7 day trial and then they start charging you \$50 a month for access to course content. This kind of stinks especially if you're like me and likely to forget that you subscribed to something like this.

If you want to keep the lectures and course notes and don't care about completing a certificate or doing the group activities coursera-dl can help you archive lectures and materials for you to use later which I've done with CalArts's Graphic Design Specialization.

Same grammar as edx-dl applies here.

```
coursera-dl -u user_email_address -p user_password link_to_coursera_course_you_signed_up_for
```

This should do the same thing as edx-dl. **Don't forget to unsubscribe from your coursera course unless you want to lose *$50* a month!**


This has been a part of my *How to Research Almost Anything* blog series. Check out the links below and be sure to follow me [@timothystiles](https://twitter.com/TimothyStiles) on twitter to get updates about my latest posts!

## Conclusion
This has been a part of my *How to Research Almost Anything* blog series. Check out the links below and be sure to follow me [@timothystiles](https://twitter.com/TimothyStiles) on twitter to get updates about my latest posts!

1. [How to download tutorials and course material from youtube, edx, and coursera.](01-download-moocs.md)
2. [How to find almost any book with libgen and the gutenburg project.](02-find-almost-any-book.md)
3. [How to access almost any scientific article with sci-hub, unpaywall, and the openaccess button.](03-access-almost-any-scientific-paper.md)

how-to-research-almost-anything © by Timothy Stiles

how-to-research-almost-anything is licensed under a Creative Commons Attribution-ShareAlike 4.0 International License.
You should have received a copy of the license along with this work. If not, see http://creativecommons.org/licenses/by-sa/4.0/.