# anse.garden

The website for [@ansegarden](https://www.instagram.com/ansegarden/).

The name types itself and a garden grows out of its letters. Birds drop in and sit on the roses. Every four seconds the page cuts between a white look and a beige look, and all of it is drawn in ASCII characters.

## Credits

- The growing garden is a remix of [Type Garden](https://type-garden.vercel.app) by Akshat Agarwal, rebuilt from the source he shares for making your own version.
- The ASCII character set comes from [ascii-magic-art](https://www.ascii-magic.com) (MIT License, Copyright (c) 2026 ASCII Magic).
- The type is Playfair Display and DM Mono from Google Fonts (SIL Open Font License).

## The portfolio

The PORTFOLIO button opens a plain ASCII box of 18 equal squares: 6 across and 3 down on a wide screen, 3 across and 6 down on a phone. Each square holds a piece of work as a moving GIF or a looping video. Tapping one shows it full screen, with a link to its Instagram post.

To add work:

1. Put the file in `work/`. A looping MP4 plays just like a GIF and is much smaller.
2. Add it to `posts.json`. The first entry goes in the first square. `how` is the one line shown under it full screen; leave `url` out until it's posted and it links to the profile:

   ```json
   [
     { "media": "work/first-post.mp4", "url": "https://www.instagram.com/p/XXXXXXXXXXX/", "title": "First post", "how": "js + webgl + z → z² + c" }
   ]
   ```

3. Commit and push. The first 18 entries fill the squares.

To try a list without publishing it, open the page with `?posts=` followed by the path to another JSON file.

## Run it locally

```
python3 -m http.server 4620
```

Then open http://localhost:4620. Add `?ascii=0` to see it without the ASCII effect, or `?hold&look=beige` to stay on one look.
