# anse.garden

The website for [@anse.garden](https://www.instagram.com/anse.garden/).

The name types itself and a garden grows out of its letters. Birds drop in and sit on the roses. Every four seconds the page cuts between a white look and a beige look, and all of it is drawn in ASCII characters.

## Credits

- The growing garden is a remix of [Type Garden](https://type-garden.vercel.app) by Akshat Agarwal, rebuilt from the source he shares for making your own version.
- The ASCII character set comes from [ascii-magic-art](https://www.ascii-magic.com) (MIT License, Copyright (c) 2026 ASCII Magic).
- The type is Playfair Display and DM Mono from Google Fonts (SIL Open Font License).

## Run it locally

```
python3 -m http.server 4620
```

Then open http://localhost:4620. Add `?ascii=0` to see it without the ASCII effect, or `?hold&look=beige` to stay on one look.
