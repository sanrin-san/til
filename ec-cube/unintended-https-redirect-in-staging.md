# ステージング環境での意図しないhttpsリダイレクト

`.env`は以下になっているが、`mypage`や`admin`がhttpsになってしまう

```
ECCUBE_FORCE_SSL=0
```

よくわからないが解決。キャッシュ？  
  
最終的にチェックした場所

```
Eccube\DependencyInjection;
```

