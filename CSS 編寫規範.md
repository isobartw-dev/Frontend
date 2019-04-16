# CSS 編寫規範


## selector

### 禁止使用
- HTML tag  
   除了reset、base、CMS editor  
   *editor 的設定會用 editor 作為父元素名稱，再向下指定各個 HTML 樣式*
- id


## BEM

### block - 獨立的元件、區塊、元素

`header` `footer` `nav` `form` `btn`

### element - block 內的元素

用 `-` 連接 block，只能有一層  
`header-logo` `footer-logo` `nav-item`

### modifier - 標示 block、element 不同的狀態或樣式

用 `--` 連接 block 或 element  
`header--black` `footer-logo--small`

最多可以到兩層，第一層為修飾名稱，第二層為修飾值  
`header--theme--light`

### nameSpace - 全站樣式設定

`text-` `bg-` `icon-`

**js hook**：`is-` `js-`

### Mixes 方法
BEM 提供此方法為避免重複編寫相同樣式  
[原文說明](https://en.bem.info/methodology/css/#mixes)

#### 一個 HTML 元素可結合不同樣式  
透過 block-element 的方式設定 HTML 元素的間隔及定位  
```
<header class="header">
    <button class="button header-button">...</button>
</header>
```
#### 一個樣式應用在不同的 HTML 元素
```
<article class="article text">...</article>

<footer class="footer">
    <div class="copyright text">...</div>
</footer>
```
## format
 - prettier

## lint
### stylelint
- stylelint-config-sass-guidelines
  - max-nesting-depth: 2
  - selector-pseudo-class-no-unknown: true,
  - selector-max-type: 0,
  - selector-max-pseudo-class: 2,
  - selector-class-pattern: null,
- stylelint-selector-bem-pattern
### eslint
- eslint-config-standard
