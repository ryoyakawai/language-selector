# language-selector (Polymer Element)

This is the Polymer element that allow you to add language selector on your web page. This element would make rid of  these problems:

- To prepare multiple HTML file for each languages for those are supported by your web page
- To deal with implementing language selector for each web page
- To take long loading time to display another page which is written in aother languages with exactlly same layout and content


# Live Demo
[Demo](https://ryoyakawai.github.io/language-selector/)


# Useage
To use this element:

- 2 lines for preparing
- write <youtube-play></youtube-play> tag and adding attributes, that is explained in below, in it.

## Prepareing
````html
<script src="https://polygit.org/components/webcomponentsjs/webcomponents-loader.js"></script>
<link rel="import" href="language-selector.html">
````

## Write content with multiple language within same layout

Two steps are required to ready to go!

### Set Language Selector
To display a language selector, werite `language-selector` HTML tag below with several attribute:

````html
<language-selector deflang="ja" langs="en:ja" switcher></language-selector>
````
#### Attributes

- **deflang** : Default language that the page wants to provide when user is landed the page
- **langs** : The languages that are providing in this page


### Write content
Translated contents of block must be located inside of `language-selector` tag.
And contents must be specify language by `lang` attribute and class name `translation` must be specified.
````html
<language-selector>
  <span class="translation" lang="ja">
  日本語ページです。ここに日本語でページのコンテンツを書いていきます。<br>
  画像、動画等の言語に依存しないであろうコンテンツは2度書く必要はありません。
  </span>
  <span class="translation" lang="en">
  This is the page in English. Write page content here in English.<br>
  The contents those are not making difference depending on language does not need to write twice.
</span>
</language-selector>
````

### Known issues
- Do not work properly when `language-selector` tag are located in different DOM tree.

### Attributes
- **lang** : Specify language

# License
Apache 2.0

