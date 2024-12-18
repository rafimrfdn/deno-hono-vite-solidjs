# Deno + Hono + Vite + SolidJS

Tutorial from [deno example SolidJS](https://deno.com/blog/build-solidjs-with-deno)  

> Make sure to install Deno 2.1 or later, I am using Deno 2.1.4 here.

## Usage

### install dependencies

```bash
$ deno install
```
Runs the app in the development mode.<br>
Open [http://localhost:5173](http://localhost:5173) to view it in the browser.

### run for development

```bash
$ deno task dev
```

### build the app for production

```bash
$ deno task build
```

### serve locally

after build the app, you have to run 2 thing in the terminal (api and the built app)

1. run the api

```bash
$ deno task dev:api
```
it will run the Hono app on [http://localhost:8000](http://localhost:8000) as backend.

2. run the app

```bash
$ deno task preview
```
Open [http://localhost:4173](http://localhost:4173) to view it in the browser.

> note do not use preview on production (vps), but your own web server (nginx, apache, etc) to serve the app.
