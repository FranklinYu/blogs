# 我的代碼哲學

- 對於未列出的語言、系統，默認使用[谷歌的標準](https://github.com/google/styleguide)。
- 在獨立腳本中使用 [Shebang](http://zh.wikipedia.org/wiki/Shebang_(Unix)) 。

## C/C++

- [C coding standard](https://users.ece.cmu.edu/~eno/coding/CCodingStandard.html)
- [Tabs for indentation, spaces for alignment](http://stackoverflow.com/a/8769873).
- 函數返回值使用 `<cstdlib>` 中的巨集 `EXIT_SUCCESS` 或 `EXIT_FAILURE`。
- 使用 `Makefile`；如果有GNU make，使用
  [implicit rules](https://www.gnu.org/software/make/manual/html_node/Implicit-Rules.html).
- 編譯選項
    - 開發模式：`-g`
    - GCC：`-Wall -Wextra -pedantic -Wcast-qual`
        - 生產模式：`-O3`
        - C++：`-std=c++11`

## Ruby

- 參考 [GitHub Ruby 指南](https://github.com/styleguide/ruby)，（Juanito Fatas翻譯的）[Ruby 社羣指南](https://github.com/JuanitoFatas/ruby-style-guide/blob/master/README-zhTW.md) 和 [Rails 社羣指南](https://github.com/JuanitoFatas/rails-style-guide/blob/master/README-zhTW.md)。
- [RSpec 指導](http://betterspecs.org/zh_tw/)
- 在 `Gemfile` 中用 `~>` 固定 gem 的版本。

## Python

- 參考 [Github](https://www.python.org/dev/peps/pep-0008/) 。

## Git

- [一个成功的 Git 分支模型](http://www.oschina.net/translate/a-successful-git-branching-model)
