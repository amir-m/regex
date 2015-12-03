# regex

```javascript
  function findQuote(text) {
    //console.log(text);
    var q = text.match(/>>\s*\w.*\n*/g);
    // return console.log(q);
    if (q) {
      for (var i in q) {
        q[i] = q[i].replace(/\s*$/, '');        
      }
    }
    return q;
  }
  
  function findBold(text) {
    var b = text.match(/\*\w*\*/g)
    return b;
  }
  
  function findItalic(text) {
    var i = text.match(/^_\s*\w.*_$/g);
    return i;
  }
```
