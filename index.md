## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/TinaYanUK/JavaScript-Notes/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### JavaScript Notes
Array.prototype.slice()
Const [a,b,...arr]=source;

Deconstructing 的时候可以不需要都写全所有的parameter


### JavaScript Promise
```markdown
const myPromise = new Promise((resolve, reject) => {

});

myPromise.then(result=> {  }) //resolve成功情况下
myPromist.catch(error => { }) //reject fail情况下
```

### Regular Expressions:
```markdown
Let aString = “ccccccc”;
Let bRegex =/xx|xx/i;
Let result =  bRegex.test(aString); //return true or false
```

.match()
```markdown
"Hello, World!".match(/Hello/);// Returns ["Hello"]let ourStr = "Regular expressions";let ourRegex = /expressions/;
ourStr.match(ourRegex);// Returns ["expressions"]

Note that the .match syntax is the "opposite" of the .test method you have been using thus far:
'string'.match(/regex/);/regex/.test('string');
To search or extract a pattern more than once, you can use the g flag.
let testStr = "Repeat, Repeat, Repeat";
let repeatRegex = /Repeat/g;
testStr.match(repeatRegex);// Returns ["Repeat", "Repeat", "Repeat"]
The wildcard character . will match any one character. The wildcard is also called dot and period.
let humStr = "I'll hum a song";let hugStr = "Bear hug";let huRegex = /hu./;
huRegex.test(humStr); // Returns true
huRegex.test(hugStr); // Returns true
You can search for a literal pattern with some flexibility with character classes. Character classes allow you to define a group of characters you wish to match by placing them inside square ([ and ]) brackets.
let bigStr = "big";let bagStr = "bag";let bugStr = "bug";let bogStr = "bog";let bgRegex = /b[aiu]g/;
bigStr.match(bgRegex); // Returns ["big"]
bagStr.match(bgRegex); // Returns ["bag"]
bugStr.match(bgRegex); // Returns ["bug"]
bogStr.match(bgRegex); // Returns null
to match lowercase letters a through e you would use [a-e].
let catStr = "cat";let batStr = "bat";let matStr = "mat";let bgRegex = /[a-e]at/;
catStr.match(bgRegex); // Returns ["cat"]
batStr.match(bgRegex); // Returns ["bat"]
matStr.match(bgRegex); // Returns null
/[0-5]/ matches any number between 0 and 5, including the 0 and 5.
Also, it is possible to combine a range of letters and numbers in a single character set.
let jennyStr = "Jenny8675309";let myRegex = /[a-z0-9]/ig;// matches all letters and numbers in jennyStr
jennyStr.match(myRegex);
```

### negated character sets.
For example, /[^aeiou]/gi matches all characters that are not a vowel. Note that characters like ., !, [, @, / and white space are matched - the negated vowel character set only excludes the vowel characters.

Match Characters that Occur One or More Times
For example, /a+/g would find one match in "abc" and return ["a"]. Because of the +, it would also find a single match in "aabc" and return ["aa"].

If it were instead checking the string "abab", it would find two matches and return ["a", "a"] because the a characters are not in a row - there is a b between them. Finally, since there is no "a" in the string "bcd", it wouldn't find a match.

Match Characters that Occur Zero or More Times
The character to do this is the asterisk or star: *.
```markdown
let soccerWord = "gooooooooal!";let gPhrase = "gut feeling";let oPhrase = "over the moon";let goRegex = /go*/;
soccerWord.match(goRegex); // Returns ["goooooooo"]
gPhrase.match(goRegex); // Returns ["g"]
oPhrase.match(goRegex); // Returns null
```

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/TinaYanUK/JavaScript-Notes/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
