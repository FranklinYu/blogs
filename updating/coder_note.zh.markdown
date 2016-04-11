# 程序員筆記

* 腳本中的多行字符串：[Here 文檔](http://zh.wikipedia.org/zh-hant/Here%E6%96%87%E6%A1%A3)
* Ruby：`attr_accessor != attr_reader + attr_writer`。前者定義了其他的 access 方式，比如 `<<`。
* [棄用 `web_steps.rb`](http://aslakhellesoy.com/post/11055981222/the-training-wheels-came-off)
* Minify
* Rails 應用程序服務器
	* 在 PaaS 上，使用 PaaS 推薦的軟件，如 Heroku 推薦 Puma；
	* 在 VPS（IaaS）上，使用 Phusion Passenger，因爲 Puma 需要 nginx 或者「阿帕奇」作負載均衡器，但 Phusion Passenger 本身嵌入在 nginx 中。
	* 參考：
		* [Puma vs. Phusion Passenger][Phusion]
		* [A Comparison of (Rack) Web Servers for Ruby Web Applications][DigitalOcean]
		* [Rails Server Throwdown: Passenger, Unicorn or Puma?][Engine Yard Article]
		* [App Server Arena: Part 1, A Comparison of Popular Ruby Application Servers][Engine Yard Blog]
* 正確的 range 形式是半開區間 [a, b)；如果是 N 個數，應該是 [0, N) 而不是 [1,
  N+1)。參考 [Dijkstra 的筆記][EWD831]。

[Phusion]: https://github.com/phusion/passenger/wiki/Puma-vs-Phusion-Passenger "Passenger Wiki at GitHub"
[DigitalOcean]: https://www.digitalocean.com/community/tutorials/a-comparison-of-rack-web-servers-for-ruby-web-applications "DigitalOcean"
[Engine Yard Article]: https://www.engineyard.com/articles/rails-server "Engine Yard"
[Engine Yard Blog]: https://blog.engineyard.com/2014/ruby-app-server-arena-pt1 "Engine Yard"
[EWD831]: https://www.cs.utexas.edu/users/EWD/transcriptions/EWD08xx/EWD831.html

## 多態（多型）的定義

* 特設多態（ad hoc polymorphism）：同一函數名，不同的參數給出不同的實現。比如 `add(Integer i, Integer j)` 和 `add(String i, String j)`。語言特性：函數重載，算子重載。
* 參數多態（parametric polymorphism）：同一函數名，不同的參數給出同樣的實現。比如 `add(Integer i, Integer j)` 和 `add(Double i, Double j)`（會被抽象成 `add(T i, T j)`）。語言特性：泛型，模板。
* 子類（subtyping，subtype polymorphism，inclusion polymorphism）：同一函數名，不同的調用對象給出不同的實現。語言特性：子類
