# Comentarismo

Hugo static site for Comentarismo - comment analytics and moderation platform.

The site is generated from Hugo templates, content files, and Bootstrap Material Design components.

## Requirements

- Hugo Extended
- GNU Make

Check your Hugo installation with:

```bash
hugo version
```

## Development

Start the local server:

```bash
make start
```

Build the production site:

```bash
make build
```

Clean generated output:

```bash
make clean
```

## Available Make Targets

- `make start` runs `hugo server`
- `make start-watch` aliases `make start`
- `make watch` aliases `make start`
- `make build` generates the site into `public/`
- `make clean` removes generated Hugo output

## Project Structure

- [`config/_default/`](./config/_default/) Hugo configuration
- [`config/_default/menus.en.toml`](./config/_default/menus.en.toml) main navigation menu
- [`content/`](./content/) page content files
- [`layouts/`](./layouts/) Hugo templates and partials
- [`layouts/partials/`](./layouts/partials/) reusable template components (head, menu, footer, sidemenu)
- [`static/admin-dist/`](./static/admin-dist/) Bootstrap Material Design CSS and JavaScript assets

## Site Routes

- `/` - Admin Dashboard (Material Design component showcase)
- `/login/` - Login page
- `/signup/` - Signup form (PRO plan by default)
- `/payment/` - Payment selection page
