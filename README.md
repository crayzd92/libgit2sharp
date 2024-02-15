# LibGit2Sharp

[![No Maintenance Intended][no-maint-badge]][no-maint-tech]

[no-maint-badge]: http://unmaintained.tech/badge.svg
[no-maint-tech]: http://unmaintained.tech/

**THIS REPOSITORY IS NOT ACTIVELY MAINTAINED**

 - Updated to [0.26.2] of the original library
 - Forked from [Zoxive/libgit2sharp][zoxive-libgit2sharp]
 - Includes refdb implemenation for use with database-based git systems
 - Original library [libgit2sharp/libgit2sharp][og-libgit2sharp]

[0.26.2]: https://github.com/libgit2/libgit2sharp/releases/tag/v0.26.2
[zoxive-libgit2sharp]: https://github.com/zoxive/libgit2sharp
[og-libgit2sharp]: https://github.com/libgit2sharp/libgit2sharp

**LibGit2Sharp brings all the might and speed of [libgit2][libgit2], a native Git implementation, to the managed world of .NET and Mono.**

 [libgit2]: http://libgit2.github.com/

## Prerequisites

 - **Windows:** .NET 4.8.1+, .NET Standard 2.1+
 - **Linux/Mac OS X:** Mono 5.4+

## Online resources

 - [NuGet package][nuget] (Requires NuGet 2.7+)
 - [Source code][source]

 [nuget]: http://nuget.org/List/Packages/LibGit2Sharp
 [source]: https://github.com/libgit2/libgit2sharp/

## Troubleshooting and support

 - Usage or programming related question? Post it on [StackOverflow][so] using the tag *libgit2sharp*
 - Found a bug or missing a feature? Feed the [issue tracker][tracker]
 - Announcements and related miscellanea through Twitter ([@libgit2sharp][twitter])

 [so]: http://stackoverflow.com/questions/tagged/libgit2sharp
 [tracker]: https://github.com/libgit2/libgit2sharp/issues
 [twitter]: http://twitter.com/libgit2sharp

## Quick contributing guide

 - Fork and clone locally
 - Create a topic specific branch. Add some nice feature. Do not forget the tests ;-)
 - Send a Pull Request to spread the fun!

More thorough information available in the [wiki][wiki].

 [wiki]: https://github.com/libgit2/libgit2sharp/wiki

## Optimizing unit testing
LibGit2Sharp strives to have comprehensive and robust unit test suite to insure the quality of the software and to assist new contributors and users who can use the tests as sample to jump start development. There are over one-thousand unit-tests for LibGit2Sharp, this number will only grow as functionality is added.

You can do a few things to optimize running unit-tests on Windows:

1. Set the `LibGit2TestPath` environment variable to a path in your development environment.
  * If the unit-test framework cannot find the specified folder at runtime, it will fall back to the default location.
2. Configure your anti-virus software to ignore the `LibGit2TestPath` path.
3. Install a RAM disk like [IMDisk](http://www.ltr-data.se/opencode.html/#ImDisk) and set `LibGit2TestPath` to use it.
  * Use `imdisk.exe -a -s 512M -m X: -p "/fs:fat /q /v:ramdisk /y"` to create a RAM disk. This command requires elevated privileges and can be placed into a scheduled task or run manually before you begin unit-testing.

## Authors

 - **Code:** The LibGit2Sharp [contributors][committers]
 - **Logo:** [Jason "blackant" Long][blackant]

 [committers]: https://github.com/libgit2/libgit2sharp/contributors
 [blackant]: https://github.com/jasonlong

## License

The MIT license (Refer to the [LICENSE.md][license] file)

 [license]: https://github.com/libgit2/libgit2sharp/blob/master/LICENSE.md
