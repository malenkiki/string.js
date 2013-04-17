string.js
=========

A little extension to standard `String` object in JS from various scripts I have found


Few methods, just `String#md5()`, `String#sprintf()`, `String#utf8Encode()`, `String#utf8Decode()`, `String#ucword()` and `String#removeDiacritic()` taken from <https://github.com/kvz/phpjs> for many of them but unlike this team, I use prototyping in place of simple functions. So, some examples to understand:

    var s = 'This is a %s tool! I want %d others!'.sprintf('great', 2)
    console.log(s) // 'This is a great tool! I want 2 others!'

    var s = 'I love U'.md5()
    console.log(s) // '1df7ee49786c480c27f1f20ef937feae'

    var s = 'this is a sentence'.ucword()
    console.log(s) // 'This Is A Sentence'

    var s = 'écrire'.removeDiacritic()
    console.log(s) // 'ecrire'

Dual licence MIT/GPL in the same way of <https://github.com/kvz/phpjs>
