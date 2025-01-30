# wp_kses()

[wp_kses](https://developer.wordpress.org/reference/functions/wp_kses/)

指定した特定の HTMLタグ以外を除去します。

## example

```
wp_kses($content, wp_kses_allowed_html( 'post' ));
```

## wp_kses_allowed_html()

[wp_kses_allowed_html](https://developer.wordpress.org/reference/functions/wp_kses_allowed_html/)

指定されたコンテキストで許可されたHTMLタグや属性の配列を返す。

## example

```
// postで許可されたものを返す
wp_kses($content, wp_kses_allowed_html( 'post' ));
```

# wp_kses_post()

[wp_kses_post](https://developer.wordpress.org/reference/functions/wp_kses_post/)

```
// 同様の処理
wp_kses_post($content)
wp_kses($content, wp_kses_allowed_html( 'post' ));
```
