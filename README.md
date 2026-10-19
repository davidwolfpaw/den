# The Den

Small projects and experiments by david wolfpaw, hosted at **https://den.david.garden**.


## Everything here is yours to use

Take any of it, fork, reuse, whatever. Just share with others!

- **Code**: [MIT](LICENSE). Keep the copyright line, do what you like.
- **Writing, images, and other content**: [CC BY-SA 4.0](LICENSE-CONTENT) ([summary](https://creativecommons.org/licenses/by-sa/4.0/)). Credit and share what you build on it under the same terms.

If something here is useful to you, I wanna know! Feel free to message me to share!

## Notes to self

**Layout:** One folder per project, served straight from `main`:

```
den/
├── index.html          # redirects to david.garden; there is no project index
├── CNAME               # custom domain
├── .nojekyll           # serve files as-is; without it Jekyll eats _folders and {{ braces }}
└── my-project/
    └── index.html
    └── style.css
    └── script.js
```

**Adding one:** Make a folder (lowercase, hyphens), put an `index.html` in it, push to `main`. Live at `https://den.david.garden/my-project/` a minute later.


## Conventions (Reminders to Myself)

- **Relative paths:** Use `./style.css`, not `/style.css`, so a project works from any folder if moved.
- **Prefix storage keys:** All projects share one origin, so `localStorage` is shared. Use keys like `my-project:highscore`, not `highscore`.
- **Nothing secret:** This repo is public, and so is its full history. No API keys, tokens, or private data.
- **Preview locally:** Run `python3 -m http.server` in the repo root and visit http://localhost:8000/my-project/. Opening a file directly with `file://` breaks `fetch()` and other same-origin requests.
