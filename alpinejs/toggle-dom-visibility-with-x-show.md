# x-showによるDOM 要素の表示切り替え

https://alpinejs.dev/directives/show

```html
<div x-data="{ activeId: 1 }">
    <!-- Toggle Button -->
    <button
        x-on:click="activeId = 1"
        :class="activeId === 1 ? 'is-active' : ''"
        :aria-pressed="activeId === 1"
        aria-controls="content-1"
        >
        Toggle 1
    </button>
    <button
        x-on:click="activeId = 2"
        :class="activeId === 2 ? 'is-active' : ''"
        :aria-pressed="activeId === 2"
        aria-controls="content-1"
        >
        Toggle 2
    </button>

    <!-- Content -->
    <div
        id="content-1"
        x-show="activeId === 1"
        x-transition:enter.duration.200ms
        x-cloak>
        Content 1
    </div>
    <div
        id="content-1"
        x-show="activeId === 2"
        x-transition:enter.duration.200ms
        x-cloak>
        Content 2
    </div>
</div>
```

## `x-cloak`で隠す場合

```css
[x-cloak] {
    display: none;
}
```
