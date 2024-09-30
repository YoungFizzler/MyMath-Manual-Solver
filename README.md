## MyMath Static Scode Gen ##

This repo is the sourcecode for my Static website hosted on https://Mymath.AutoAce.Su which provides a manual way to manipulate a MyMath homework score request.

So how do we generate the Scode?

``` javascript
function generateScode(authCode, taskId, q1Score, q2Score) {
            var scode = authCode * taskId;
            scode = scode + q1Score * 100 + q2Score;
            scode = scode * 10000;
            scode = scode + taskId * taskId;
            return scode;
```

This function to generate the Scode takes 4 inputs; Authcode, taskid, q1score, q2score.
These inputs can be extracted by following the steps on the website.


## Getting Started ## 

Clone the repo
```
git clone https://github.com/YoungFizzler/MyMath-Manual-Solver.git
```

Cd into the Repo
```
cd MyMath-Manual-Solver
```

then simply run the file with
```
index.html
```
