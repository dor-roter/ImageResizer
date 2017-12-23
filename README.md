# ImageResizer

Use
------
  ```javascript
  var resizer = new ImageResizer({properties});
  
  resizer.resize(<img>, function(resized){
    <callbak>
  });
  ```
  
 Options
 ------
 | Option   | Type | Description                                                                   |
 |----------|------|-------------------------------------------------------------------------------|
 |quality   |int   | required compression quality, the higher the better. <br> value between 0-1.  |
 |dataurl   |Bool  | should the returned resized file be a dataurl string.                         |
 |maxHeight |int   | The maximun image height allowed by the resizer.                              |
 |maxWidth  |int   | The maximun image width allowed by the resizer.                               |
 |supported |Array | An array of strings specifing the allowed file types.                         |
 
 Errors
 -------
- **Compatibility error** - In case of canvas not being supported by the browser, the constructor method will throw this error.
