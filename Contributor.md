# JavaScript
## create a .times function. Very useful!
```javascript
function glassdoorStarGenerate(rating) {
      var fractional = rating % 1;
      var fulls = Math.floor(rating);
      var empties = 5 - fulls - 1;
      var s = '';
      var star = "<i class='fa fa-star'></i>";
 
      fulls.times(function() {
        s += "<span class='star-full'<i></i>" + star + "</span>";
      });
 
      //fractional star
      if (fractional > 0) {
        s += "<span class='star-fraction'><i style='width:" + (fractional * 100) + "%'></i>" + star + "</span>";
      }
 
      empties.times(function() {
        s += "<span class='star-empty'<i></i>" + star + "</span>";
      });
 
      return s
    }
 
    // .times function
    Number.prototype.times = function(val) {
      var i = -1;
      while (++i < this) {
        val(i);
      }
      return +this;
    }
    ```
