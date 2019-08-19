# Victor的第一個網站

## 介紹

嗯...網站！

## 使用技術

名稱    |    說明
-------|-----------
Python | 好棒!
Flask  | 好棒棒!
repl.it | 好棒棒棒!
Heroku | 好棒棒棒棒!
Github | 好棒棒棒棒棒!

## 範例代碼

```python
@app.route("/")
def root():
  ds = glob.glob("articles/*")
  result = []
  for d in ds:
    fs = glob.glob(d + "/*.txt")
    t = (d.split("/")[-1], len(fs))
    result.append(t)
  return render_template("index.html", d = result)
```

## 網址

[請點我](https://https://victordiary.herokuapp.com//)
