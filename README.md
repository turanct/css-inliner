css-inliner CLI tool
=================================================

A command line tool of [Tijs Verkoyen's Css To Inline Styles](https://github.com/tijsverkoyen/CssToInlineStyles), so that we can use it in builds.


Installation
-------------------------------------------------

### Globally

```bash
git clone https://github.com/turanct/css-inliner.git /usr/local/css-inliner && cd /usr/local/css-inliner && curl -sS https://getcomposer.org/installer | php && php composer.phar install && ln -s /usr/local/css-inliner/css-inliner /usr/local/bin/css-inliner && cd -
```

### Locally in a php project

```json
{
    "require-dev": {
        "turanct/css-inliner": "dev-master"
    },
    "config": {
        "bin-dir": "bin"
    }
}
```


Usage
-------------------------------------------------

### See USAGE message:

```bash
/path/to/css-inliner --help
```

### Inline some CSS from a file

```bash
/path/to/css-inliner file.html
```

### Inline some CSS from STDIN

```bash
cat file.html | /path/to/css-inliner
```

### Writing to a file

If you want to write to a file, you can just redirect the STDOUT to a file:

```bash
cat file.html | /path/to/css-inliner > inlined.html
```


Thanks
-------------------------------------------------

@tijsverkoyen


License
-------------------------------------------------

This code is provided under the MIT license.
