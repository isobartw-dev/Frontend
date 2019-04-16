# sass資料夾結構

使用 7-1 pattern，以下為樹狀結構範例(非專案檔案)

```
sass/
|
|– utilities/
|   |– variables.scss    // Sass Variables
|   |– functions.scss    // Sass Functions
|   |– mixins.scss       // Sass Mixins
|
|– base/
|   |– reset.scss        // Reset/normalize
|   |– text.scss         // Typography rules
|
|– components/
|   |– buttons.scss      // Buttons
|   |– carousel.scss     // Carousel
|
|– layout/
|   |– navigation.scss   // Navigation
|   |– grid.scss         // Grid system
|   |– header.scss       // Header
|   |– footer.scss       // Footer
|   |– forms.scss        // Forms
|
|– pages/
|   |– home.scss         // Home specific styles
|   |– about.scss        // About specific styles
|   |– contact.scss      // Contact specific styles
|
|– themes/
|   |– theme.scss        // Default theme
|   |– admin.scss        // Admin theme
|
|– vendors/
|   |– bootstrap.scss    // Bootstrap
|   |– jquery-ui.scss    // jQuery UI
|

css/
|– style-edit.scss       // Main Sass file
```

## 資料夾用法

### utilities

**SASSScript**：variables、mixins、functions、config files，這些檔案是作為模組化 CSS 用並沒有辦法編譯為 CSS

### base

**版面標準樣式**：reset、text、color、animation(大量使用的)或是定義一些 HTML element 的基本樣式

### layout

**版面框架**：header、footer、sidebar、navgation、breadcrumbs，還有像是 grid 或是 form 也都是屬於此類

### components

**元件、模組**：carousel、tab、accordion，獨立且可以重複使用的小區塊，檔案最多的地方

### pages

**頁面特定樣式**：像是首頁可能會是一個獨特的設計

### themes

**版面主題樣式**：某些專案可能會有此規劃，大部分可能會是不同配色的樣式

### vendors

**第三方套件樣式**：owl-carousel、colorbox...
