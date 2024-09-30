# MyMath Static Scode Gen #

This repo is the sourcecode for my Static website which provides a manual way to manipulate a MyMath homework score request.

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

## Hosting with a Domain ##

To host with a domain, Upload the Static Website folder to your hosting provider.

### Cloudflare ###

1. Fork this repo
2. Navigate to Workers and Pages on cloudflare. (*** Optional ***)
3. Click on Pages then Create.
4. Create a new page and upload the Static Website folder or login to github and use your repo.
