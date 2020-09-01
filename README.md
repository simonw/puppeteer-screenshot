# puppeteer-screenshot

Vercel app for taking screenshots of web pages using Puppeteer

Original code by [@styfle](https://github.com/styfle) in [this pull request](https://github.com/vercel/now-examples/pull/207).

I upgraded the code to work with the latest Vercel and added a `?key=` mechanism to protect it from unauthorized access.

## Usage

Set a Vercel secret called `SECRET_KEY` with a random string in it (I generated mine by running `uuidgen | md5`), then deploy.

You can access screenshots for pages using:

    https:/.../zeit.co/blog?type=png&key=...

Screenshots can take several seconds to generate so it's a good idea to cache them somewhere.
