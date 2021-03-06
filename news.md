## News

> (most recent first)

* `15th of August 2015`

1.2.7 release - a really quick release this time! That's because the previous release, 1.2.6, unfortunately missed
adding support for documentation annotations (@Ignore, @Issue, @See, @Title, @Narrative). Support for all of these 
annotations have been added in this release (the release notes have been amended to reflect this).

As usual, this release also includes some tiny bug fixes... and template reports are now easier to write.

* `12th of August 2015`

1.2.6 release - this release brings support for **parallel builds**. Until now, individual specification reports would
be created just fine, but the aggregated report would only contain the specifications run by the last Thread of a
parallel build. After this release, that is no longer the case!

Other minor improvements were also included in this release, check the release notes for details.

**BREAKING CHANGE**: for users of template reports, a necessary breaking change had to made: in Specification report
templates, to iterate over features you must now call method `eachFeature` instead of `forEach`. This was necessary
 because the old name conflicted with a native method when using Java 8. Sorry for the inconvenience.

* `8th of March 2015`

1.2.5 release - added support for [Spock 1.0](http://spockframework.github.io/spock/docs/1.0/release_notes.html),
which has been released, finally!!
Also, but not less important, now spock-reports has support for templates! This lets you make your report look
like whatever you want!

* `14th of February 2015`

1.2.4 released - some nice new features included, such as Table of Contents.

* `08th of November 2014`

1.2.3 released - downgraded minimum Groovy version required to 2.0.8 (benefits some Grails users).

* `03rd of November 2014`

Small feature release (1.2.2): added support for @Unroll-ing variables not only in Spec names,
but also in block texts (given, when, then...)

* `01st of November 2014`

Bug fix release, 1.2.1. Fixed problems with bad-behaving Specification setup methods and
removed usage of some Groovy features to allow running spock-reports with any recent JDK 7 or 8 version.

* `3rd of August 2014`

Release of version 1.2! This release includes full support for @Unroll,
amongst other small improvements.

* `3rd of July 2014`

After a long delay, I have finally published the 1.1 release on a public repo, thanks to @JayStGelais
contribution. So now ``spock-reports`` is available on Bintray's [JCenter](http://jcenter.bintray.com/)!

* `14th of September 2013`

Release of version 1.1 with some minor bug fixes and improvements in the information shown in reports.
Please check the release notes in the file `releases/Release_Notes.txt`.

* `6th of August 2013`

Today, I am proud to release version 1.0 of this project! I have made sure to make it as stable
as possible so that you can start reading proper reports for your Spock specifications without worries.
You can find the jar in the `releases` directory! Download it, place it in your classpath and you're done!
By default, the reports will be saved in the directory `build/spock-reports`, but you can change that if you want,
just check below.
I hope you find this project as useful as I have (I actually developed this out of my own need for it!).


I wrote a [blog post](http://software.athaydes.com/posts/writingspecificationsthatdoubleastestswithspock) about the motivation behind this project. Please check it out!
