# django-pager

## memo
djangoの`Paginator`や`Page`の様につかう。`Paginator`と違うのは最初に対象データ全件をとらずにページ遷移ごとに毎回データを取得する。`cls.objects.all()`のコストが高い時やリクエストごとに`Paginator`オブジェクトを作っている場合に使用。でも`Paginator`の方がコストが低い場合もある。
