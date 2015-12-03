# regex

```javascript
  function findQuote(text) {
    var q = text.match(/>>\s*\w.*\n*/g);
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
    var i = text.match(/_\w*_/g);
    return i;
  }
  // Replace more than one space with a single space
  // .replace(/ +/g, ' ');

  // Replace more than two return characters with two return characters
  // .replace(/\n\n\n+/g, '\n\n');
```
