Bash for Android
================

This is a series of commits on top of the [Bash Git repository](https://savannah.gnu.org/git/?group=bash)'s `master` branch to make it buildable using the Android NDK.

Building Instructions
---------------------

1. Check out the repository. If updating, make sure to use `git pull --rebase`.
2. Create a standalone NDK toolchain using the instructions provided [here](https://developer.android.com/ndk/guides/standalone_toolchain.html).
3. Run the `configure_android` script, which is a wrapper for `configure` with the proper flags.
4. Run `make`.

Note that it has only been tested using API level 24 and GCC as the compiler.