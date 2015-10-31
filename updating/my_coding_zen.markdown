> It's easier to ask forgiveness than it is to get permission.  
> -- [Grace Hopper](https://en.wikiquote.org/wiki/Grace_Hopper)

- For unlisted language, default style follows
  [Google's instruction](https://github.com/google/styleguide).
- Use [Shebang](http://en.wikipedia.org/wiki/Shebang_(Unix)) for standalone
  scripts.

## C/C++

- [C coding standard](https://users.ece.cmu.edu/~eno/coding/CCodingStandard.html)
- [Tabs for indentation, spaces for alignment](http://stackoverflow.com/a/8769873).
- Functions return with macros `EXIT_SUCCESS` or `EXIT_FAILURE` in `<cstdlib>`.
- Use `Makefile`; if GNU make is available, use the
  [implicit rules](https://www.gnu.org/software/make/manual/html_node/Implicit-Rules.html).
- Compiling options
    - Development mode: `-g`
    - GCC: `-Wall -Wextra -pedantic -Wcast-qual`
        - Production mode: `-O3`
        - C++: `-std=c++11`

## Ruby

- Refer to [GitHub](https://github.com/styleguide/ruby),
  Batsov's [Ruby](https://github.com/bbatsov/ruby-style-guide) and [Rails](https://github.com/bbatsov/rails-style-guide) style guide.
- [RSpec guides](http://betterspecs.org/)
- Fix main version of gems in `Gemfile` (with `~>`).

## Python

- Refer to [Github](https://www.python.org/dev/peps/pep-0008/)

## JavaScript

- Avoid built-in `window.prompt()`, `window.confirm()` and `window.alert()`.
  Reference:
    - [Programmers.SX](http://programmers.stackexchange.com/q/106031)
    - [ESLint Rule](http://eslint.org/docs/rules/no-alert.html)

## Git

- [A successful Git branching model](http://nvie.com/posts/a-successful-git-branching-model/)
