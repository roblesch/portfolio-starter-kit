# Portfolio Starter Kit

A [zola](https://github.com/getzola/zola) + [Tailwind CSS](https://tailwindcss.com/) port of the 
Vercel [Portfolio Starter Kit](https://vercel.com/templates/next.js/portfolio-starter-kit).

## Dependencies

- [`zola`](https://github.com/getzola/zola/releases) >= 19.0.2
- [`tailwindcss`](https://tailwindcss.com/blog/standalone-cli) >= v4.0.6

## Installation

1. Add the theme to your repository.

```sh
git submodule add https://github.com/roblesch/portfolio-starter-kit themes/portfolio-starter-kit
```

2. Add the following to your `config.toml`.

```toml
theme = "portfolio-starter-kit"

generate_feeds = true
feed_filenames = ["rss.xml"]

[extra]
github_url = "https://github.com/roblesch/zola-portfolio-starter-kit"
repo_url = "https://github.com/roblesch/zola-portfolio-starter-kit"
```

3. (Optional) Copy example pages.

```sh
mkdir -p content && cp -r themes/portfolio-starter-kit/content/* content/
```

## Run the Server

```sh
zola serve & tailwindcss -i themes/portfolio-starter-kit/templates/global.css -o public/global.css --watch
``` 

## References

[Portfolio Starter Kit](https://vercel.com/templates/next.js/portfolio-starter-kit)
