---
layout: article
titles:
  # @start locale config
  en      : &EN       About
  en-GB   : *EN
  en-US   : *EN
  en-CA   : *EN
  en-AU   : *EN
  zh-Hans : &ZH_HANS  关于
  zh      : *ZH_HANS
  zh-CN   : *ZH_HANS
  zh-SG   : *ZH_HANS
  zh-Hant : &ZH_HANT  關於
  zh-TW   : *ZH_HANT
  zh-HK   : *ZH_HANT
  ko      : &KO       소개
  ko-KR   : *KO
  fr      : &FR       À propos
  fr-BE   : *FR
  fr-CA   : *FR
  fr-CH   : *FR
  fr-FR   : *FR
  fr-LU   : *FR
  # @end locale config
key: page-about
---
# What we did

We worked various way like unify indent, compensate example, fix typo, and so on.

Below are the individual contribution of the project, team leader comes first and other member's subsequnce is 가나다순(alphabetical order).

This only listed the key contributions, and you can check all of them by clicking names or the link below.

<div>{%- assign _summary_d1 = site.data.works.example-%}</div>
## [{{ _summary_d1.realnameEN }} ({{ _summary_d1.name }})](https://20-1-skku-oss.github.io/2020-1-OSS-2/2020/06/08/What-devquint-Done.html) `Team Leader`{:.info}
<div>{%- include work-list.html userdata=_summary_d1 only_core=true-%}</div>

# Theme
![TeXt Theme](https://raw.githubusercontent.com/kitian616/jekyll-TeXt-theme/master/screenshots/TeXt-home.jpg)
- We used [TeXt Theme](https://github.com/kitian616/jekyll-TeXt-theme)!

TeXt is a super customizable Jekyll theme for personal site, team site, blog, project, documentation, etc. Similar to iOS 11 style, it has large and prominent titles, round buttons and cards.

```javascript
(() => console.log('Hello, World!'))();
```