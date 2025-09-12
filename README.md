# modern-poetry 中国现代诗和外国诗数据库

<p align="center">
  <a href="https://github.com/qyxtim/modern-poetry/blob/master/LICENSE">
    <img height="18px" alt="License" src="https://img.shields.io/badge/license-Apache%202.0-blue">
  </a>
  <a href="https://github.com/qyxtim/modern-poetry/graphs/contributors">
    <img height="18px" alt="Contributors" src="https://img.shields.io/github/contributors/qyxtim/modern-poetry.svg">
  </a>
  <a href="https://github.com/qyxtim/modern-poetry/graphs/contributors">
    <img height="18px" alt="Contributors" src="https://img.shields.io/badge/PR-welcome-green">
  </a>
</p>

---

<p align="center">
  <a href="https://github.com/qyxtim/modern-poetry">
      <img src="https://cdn.jsdelivr.net/gh/qyxtim/modern-poetry@master/logo.png" alt="chinese-poetry">
  </a>
</p>

 [Chinese_version](#Chinese_version) | [English_version](#English_version)

---

# Chinese_version

Part1: chinese-modern-poetry 中国近现代诗

最全的中国近现代诗数据库，包含约5000首中国现代诗、3000首当代诗、三万首近现代诗。数据来源于互联网。

**做这个仓库的原因：** 我本人是个爱好诗歌的人，尤其是近代诗歌。但网上却缺少一个很好的中国近代诗库，所以我便抽出了时间做了这个项目。本项目采用 json 分发数据。日后本项目会加入英语的现代诗以及稍微久远一些的诗，如莎士比亚的作品。

Part2: poetry from other countries 其它国家的诗

最全的国外诗歌数据库，包含近3万首诗歌，分别来自英国、美国、德国、俄国等其他国家。数据来源于互联网。

做这一部分是想让全球各地的人能够了解到每个地区的不同文化。如果细心看这一部分的 json 文件，可以看到有些文件里有两次作者的名字。这是因为采用了本土语言以及英语。

## 贡献

由于抓取现代诗资源的网站的布局很乱，所以现代诗的内容以及标题可能会存在有匹配错误的情况，如果发现了问题你可以提交 PR 或者通过 issue 讨论来优化这个项目。

由于本项目不止局限于中国现代诗，也欢迎英文、法文等语言的诗歌投稿。投稿的内容可以在 issue 内讨论。如果要通过PR投稿，投稿的格式一定要参考以下格式:

```
// Format of posts (not for translation)
[{
	"author":"author-name",
	"title":"poem-title",
	"paragraphs":[
	"sentence-1","sentence-2"
	]
}, ...
]

// Format of author
[{
	"name": "author-name",
	"description": "Description about author"
}, ...
]
```

如果你想要翻译本项目的诗或者找到本项目诗的合适翻译，可以通过如下格式提交：

```
// Format of posts (translation)
[{
	"author":"author-name(Chinese name)",
	"title":"poem-title",
	"translation":[
	"sentence-1","sentence-2"
	],
	"origin":"poem's origin name"
}, ...
]

// Format of author
[{
	"name": "author-name",
	"description": "Description about author"
}, ...
]
```

内容需要提交到特定语言的 translation 文件夹内。

如果你发现你想要翻译的作者已经被翻译了，但是翻译的不够好，你可以在issue里发起讨论（需要同时放上自己的翻译以及原始翻译），点赞数最高的将被收录进文件内。

注意：在PR时，请一定确保没有重复的内容。

## 词云

<details open="">
    <summary>
        中国现代诗
    </summary>
    <img src="https://cdn.jsdelivr.net/gh/qyxtim/modern-poetry@master/clouds/cloud-chinese-contemporary.png" style="max-width:100%;">
</details>

<details>
    <summary>
        中国当代诗
    </summary>
    <img src="https://cdn.jsdelivr.net/gh/qyxtim/modern-poetry@master/clouds/cloud-chinese-modern-time.png" style="max-width: 100%;">
</details>

<details>
    <summary>
        中国近代诗
    </summary>
    <img src="https://cdn.jsdelivr.net/gh/qyxtim/modern-poetry@master/clouds/cloud-chinese-modern.png" style="max-width:100%;">
</details>

<details>
    <summary>
        英文诗
    </summary>
    <img src="https://cdn.jsdelivr.net/gh/qyxtim/modern-poetry@master/clouds/cloud-English.png" style="max-width:100%;">
</details>

## 这个仓库可以拿来干什么？

这个仓库有很多的用途：

- 从最根源上来说它是一个诗歌数据库，它包含了许多国家的诗集
- 它可以用来开发一些衍生产品
	- [一言 - 中国现代诗]( https://poem.blinkstar.cn/ )
	- 基于 NLP 的现代诗歌创作
	- ......

## 许可证

[Apache](https://github.com/qyxtim/modern-poetry/blob/master/LICENSE) License

---

# English_version

**Part1**: chinese-modern-poetry

The most comprehensive database of modern Chinese poetry contains about 5,000 modern Chinese poems, 3,000 contemporary poems and 30,000 modern Chinese poems. The data comes from the Internet.

**Reasons for this repository:** I am a lover of poetry, especially modern poetry. However, there is a lack of a good library of modern Chinese poems online, so I took the time to do this project. This project USES json to distribute data. The project will include modern poetry in English as well as older poetry, such as Shakespeare in the future.

**Part2**: poetry from other countries

The most complete foreign poetry database contains nearly 30,000 poems from Britain, the United States, Germany, Russia and other countries. The data comes from the Internet.

This part is to let people from all over the world know the different cultures of each region. If you look closely at the json file in this section, you can see that some of the files have the author's name twice. This is due to the use of native languages as well as English.

## Contribution

Because the layout of websites that grab modern poetry resources is very messy, there may be matching errors in the content and titles of modern poetry. If you find problems, you can give feedback in the following by opening a PR or issue directly.

Since this project is not limited to modern Chinese poetry, poems in English, French and other languages are also welcome to submit. You can discuss your idea on issues. If you want to submit through PR, you must refer to the following format:

```
// Format of posts

[{
	"author":"author-name",
	"title":"poem-title",
	"paragraphs":[
	"sentence-1","sentence-2"
	]
}, ...
]

// Format of authors
[{
	"name": "author-name",
	"Description": "Description about author"
}, ...
]

```

If you want to translate the poetry of this project or find a suitable translation of the poetry of this project, you can submit it in the following format:

```
// Format of posts (translation)
[{
	"author":"author-name(Chinese name)",
	"title":"poem-title",
	"translation":[
	"sentence-1","sentence-2"
	],
	"origin":"poems' origin name"
}, ...
]

// Format of author
[{
	"name": "author-name",
	"description": "Description about author"
}, ...
]
```

The content needs to be submitted to a language-specific translation folder.

If you find that the author you want to translate has already been translated, but the translation is not good enough, you can initiate a discussion in issue (both your own translation and the original translation are required), and the one with the highest number of thumb up will be included in the document.

Note: in PR, please make sure there is no repetition.

## Clouds

<details open="">
    <summary>
        Chinese contemporary poem
    </summary>
    <img src="https://cdn.jsdelivr.net/gh/qyxtim/modern-poetry@master/clouds/cloud-chinese-contemporary.png" style="max-width:100%;">
</details>

<details>
    <summary>
        Chinese modern poem
    </summary>
    <img src="https://cdn.jsdelivr.net/gh/qyxtim/modern-poetry@master/clouds/cloud-chinese-modern-time.png" style="max-width: 100%">
</details>

<details>
    <summary>
        Chinese modern-time poem
    </summary>
    <img src="https://cdn.jsdelivr.net/gh/qyxtim/modern-poetry@master/clouds/cloud-chinese-modern.png" style="max-width:100%;">
</details>

<details>
    <summary>
        Poem from USA and UK
    </summary>
    <img src="https://cdn.jsdelivr.net/gh/qyxtim/modern-poetry@master/clouds/cloud-English.png" style="max-width:100%;">
</details>

## What can this repository be uessed for?

The warehouse has many USES:

- At its most basic, it is a database of poems from many countries

- It can be used to develop some derivative products
	- [Chinese Modern Poetry Sharing](https://poem.blinkstar.cn/)
	- Automatic modern poetry generator based on NLP
	- ...

## License

[Apache](https://github.com/qyxtim/modern-poetry/blob/master/LICENSE) License