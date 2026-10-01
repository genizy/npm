# HOW TO DEPLOY YOUR OWN
1. clone repo (git glone https://github.com/genizy/npm)
2. delete `gnrunner` folder and move everything in `deploy-your-own` folder to root directory
3. open RUN.py and change `name = "tuffname"` to something that you actually own on npmjs
    * If you dont have a npmjs account or package, heres how to make it:
        1. tutorial here
4. run `python RUN.py`
5. delete RUN.py
6. run `npm publish`

it should be published now