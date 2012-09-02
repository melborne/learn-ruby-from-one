!SLIDE
# １から始める<strong class='ruby' id='title'>Ruby</strong> #

!SLIDE subsection transition=fade
# Rubyの１について

!SLIDE bullets
* 数学の世界で１は数である

!SLIDE bullets
* ３歳の子供でもそれを知っている

!SLIDE bullets
* そして
* 私やあなたが老いて死にゆくまで

!SLIDE bullets
* １は数であり
* そこに疑念の入る余地はない

!SLIDE bullets
* プログラミングの世界でも
* ふつう１は数である

!SLIDE bullets
* CでもJavaでもHaskellでも
* １は数であり

!SLIDE bullets
* それ以上でも
* それ以下でもない

!SLIDE bullets
* ところが驚くべきことに

!SLIDE bullets
* <strong class='ruby'>Ruby</strong>の世界では

!SLIDE
## １は数ではないのである

!SLIDE bullets
* 嘘だと思うなら
* irbを立ち上げて
* 次のようにしてみるといい

!SLIDE commandline incremental

    $ irb
    $ 1.next
     # => 2

!SLIDE bullets
* あなたは今１に
* "next"
* というメッセージを送った

!SLIDE bullets
* そうしたら１は
* ２という答えを返したのだ

!SLIDE bullets
* つまり<strong class='ruby'>Ruby</strong>の世界で１は
* 数以上のものであり

!SLIDE bullets
* メッセージに返答する
* 「何か」である

!SLIDE bullets

* <strong class='ruby'>Ruby</strong>の世界でそれは
* 「オブジェクト」
* と呼ばれている

!SLIDE bullets
* １はメッセージに反応する
* オブジェクトである

!SLIDE

## しかしここで一つの疑問が湧いてくる

!SLIDE bullets

* それならば今
* １が返した２というのは
* 何なのか

!SLIDE bullets
* 数なのか
* それとも
* オブジェクトなのか



!SLIDE bullets
* この疑問にもirbが答えてくれる

!SLIDE commandline incremental
    $ irb
    $ 1.next.next
     # => 3

!SLIDE bullets

* １からの返答にさらに
* "next"という
* メッセージを送ってみる

!SLIDE bullets
* つまり
* "1.next"で返される２に
* メッセージを送ってみると
!SLIDE bullets
* 果たして
* ３が返ってきた

!SLIDE bullets
* そう１から返答された２も
* やはりオブジェクトだったのだ

!SLIDE bullets
* 疑い深いあなたは
* これだけでは
* 納得しないかも知れない

!SLIDE bullets
* そしてirbできっと
* 次のように
* 入力するのだろう..

!SLIDE commandline incremental commandsmall

    $ irb
    $ 1.next.next.next.next.next.next.next.next.next.next \
       .next.next.next.next.next.next.next.next.next.next \
       .next.next.next.next.next.next.next.next.next.next \
       .next.next.next.next.next.next.next.next.next.next \
       .next.next.next.next.next.next.next.next.next.next \
       .next.next.next.next.next.next.next.next.next.next \
       .next.next.next.next.next.next.next.next.next.next \
       .next.next.next.next.next.next.next.next.next.next \
       .next.next.next.next.next.next.next.next.next.next \
       .next.next.next.next.next.next.next.next.next
     # => 100

!SLIDE

# 納得した？

!SLIDE bullets
* そう
* <strong class='ruby'>Ruby</strong>の世界では
* 入り口も出口も

!SLIDE bullets
* そのすべてが
* オブジェクトなのである

!SLIDE bullets
* さて
* １がオブジェクトなら
* "next"以外の

!SLIDE bullets
* どんなメッセージに
* 反応するのかが
* 気になるところだ

!SLIDE bullets
* <strong class='ruby'>Ruby</strong>ではその答えも
* １に聞けばいい

!SLIDE bullets
* "methods"
* というメッセージを
* １に送ってみよう

!SLIDE commandline incremental commandsmall

    $ irb
    $ 1.methods
    $ => [:to_s, :-@, :+, :-, :*, :/, :em, :%, :modulo, :divmod,\
      :fdiv, :**, :abs, :magnitude, :==, :===, :<=>, :>, :>=, :<,\
      :<=, :~, :&, :|, :^, :[], :<<, :>>, :to_f, :size, :zero?,\
      :odd?, :even?, :succ, :integer?, :upto, :downto, :times,\
      :next, :pred, :chr, :ord, :to_i, :to_int, :floor, :ceil,\
      :truncate, :round, :gcd, :lcm, :gcdlcm, :numerator,\
      :denominator, :to_r, :rationalize, :singleton_method_added,\
      :coerce, :i, :+@, :eql?, :quo, :remainder, :real?,\
      :nonzero?, :step, :to_c, :real, :imaginary, :imag, :abs2,\
      :arg, :angle, :phase, :rectangular, :rect, :polar,\
      :conjugate, :conj, :between?, :nil?, :=~, :!~, :hash,\
      :class, :singleton_class, :clone, :dup, :initialize_dup,\
      :initialize_clone, :taint, :tainted?, :untaint, :untrust,\
      :untrusted?, :trust, :freeze, :frozen?, :inspect, :methods,\
      :singleton_methods, :protected_methods, :private_methods,\
      :public_methods, :instance_variables,\
      :instance_variable_get, :instance_variable_set,\
      :instance_variable_defined?, :instance_of?, :kind_of?,\
      :is_a?, :tap, :send, :public_send, :respond_to?,\
      :respond_to_missing?, :extend, :display, :method,\
      :public_method, :define_singleton_method, :__id__,\
      :object_id, :to_enum, :enum_for, :equal?, :!, :!=,\
      :instance_eval, :instance_exec, :__send__]

!SLIDE bullets

* これらは
* １が応答できる
* メッセージの集合で

!SLIDE bullets
* <strong class='ruby'>Ruby</strong>では
* 「メソッド」
* と呼ばれている

!SLIDE bullets
* つまり１は
* あなたからの問い合わせに対し
* これら130個もの
* メソッドで応答する

