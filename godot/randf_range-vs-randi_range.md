# _process()と_physics_process()の違い

## `float` randf_range(from: float, to: float)

`from` から `to` まで (両端を含む) のランダムな浮動小数点値を返します。

```
randf_range(0, 20.5) # Returns e.g. 7.45315
randf_range(-10, 10) # Returns e.g. -3.844535
```

## `int` randi_range(from: int, to: int)

`from` から `to` まで (両端を含む) のランダムな符号付き32ビット整数を返します。`to` が from より小さい場合は、入れ替えられます。

```
randi_range(0, 1)      # Returns either 0 or 1
randi_range(-10, 1000) # Returns random integer between -10 and 1000
```
