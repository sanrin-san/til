# Dockerを使用してPHPバージョンを固定

## PHP 8.2を使ったコンテナの起動

```
docker run -it --rm php:8.2 bash
```

この中でcomposer installやcomposer updateを実行すれば、常にPHP 8.2を使用できる。
