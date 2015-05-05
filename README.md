# IPFS Blog

This is the source repository for the [IPFS Blog](http://ipfs.io/blog).

## Editing

### Creatig a Post

To create a new post, use

```sh
hugo new post/<next-number>-<short-title>/index.md

# for example
hugo new post/0-hello-worlds/index.md
```

That will create a directory for the post inside `content/`. Edit the `index.md` there. Place any static assets (e.g. images) inside its mirror in

```
mkdir static/post/<next-number>-<short-title>/
```

hugo will put all of these into the same target dir (we have to do this until https://github.com/spf13/hugo/issues/147 is fixed).

### Theme Edits

There is a trivial `ipfs` theme inside `themes/`. It follows the standard hugo theme setup. It's based on [the example viewer](https://github.com/ipfs/examples/tree/master/webapps/example-viewer). Modify the files inside

```
themes/ipfs/layouts/
```
