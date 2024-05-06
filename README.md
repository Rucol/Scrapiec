## Whai I did?

The entire scrapper file, I scraped prices using BS4, searching for information using html tags. I was using there Beautiful Soup 4, html parser, requests.

# Access

Front: [https://zciwolvo.github.io/skapiec/]
API: [https://www.igorgawlowicz.pl/skapiec/get_data]

# Local startup instructions

To run the project locally, change the URL given in fetches in `skapiec/skapiec/src/app.js` in lines 15 and 16, we change:

`https://www.igorgawlowicz.pl/skapiec/scrape?phrase=${search}&page=${selectedPage}` at `http://127.0.0.1:5000/scrape?phrase=${search}&page= ${selectedPage}`

and

`https://www.igorgawlowicz.pl/skapiec/get_data?phrase=${search}` to `http://127.0.0.1:5000/get_data?phrase=${search}`

then we need to prepare two terminal windows:

we open the first one in the main repository, we must have python3 installed, then we write:

```bash
pip install -r requirements.txt

pythonserver.py
```

Now we need to open a second terminal in the path `skapiec/skapiec`, we must have `node` installed:

```bash
npm install

npm start
```

The application will run locally and we can use it from the URL in the console
