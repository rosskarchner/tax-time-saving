# Tax time saving

Landing page for tax refund insert campaign that encourages people to save their refund.


## Dependencies

- [Grunt](http://gruntjs.com): task runner for pulling in assets,
  linting and concatenating code, etc.
- [Less](http://lesscss.org): CSS pre-processor.
- [Capital Framework](https://github.com/cfpb/capital-framework):
  User interface pattern-library produced by the CFPB.
- [Sheer](https://github.com/cfpb/sheer):
  server that interprets the Jinja2 templates.


## Installation

1. Install [Node.js](http://nodejs.org) however you'd like.
2. Install [Grunt](http://gruntjs.com):

   ```bash
   npm install -g grunt-cli bower
   ```
3. Next, install the dependencies and compile the project with:

   ```bash
   ./setup.sh
   ```

   __NOTE:__ To re-install and rebuild all the site’s assets run
   `./setup.sh` again. See the [usage](#usage) section on updating all the
   project dependencies.
4. Install [Sheer](https://github.com/cfpb/sheer) by following the instructions
   in its README.


## Usage

Each time you fetch from the upstream repository (this repo), run `./setup.sh`.
This setup script will remove and re-install the project dependencies and
rebuild the site's JavaScript and CSS assets.

To watch for changes in the source code and automatically update the running site,
open a terminal and run:

```bash
grunt watch
```

Alternatively, if you don't want to run the full watch task,
there are three available sub-tasks:

```bash
# Watch & compile CSS only
grunt watch:css

# Watch & compile JS only
grunt watch:js

# Watch & compile CSS & JS only
grunt watch:cssjs
```


## How to test the software

After running `./setup.sh` or compiling with Grunt,
`cd` into `/dist` and run `sheer serve --debug`.
After it starts, visit <http://localhost:7000/> in your browser to see the site.


## Getting help

Use the issue tracker to follow the development conversation.
If you find a bug not listed in the issue tracker, please file a bug report.


## Getting involved

We welcome your feedback and contributions. See the
[contribution guidelines](https://github.com/cfpb/open-source-project-template/blob/master/CONTRIBUTING.md)
for more details.

Additionally, you may want to consider
[contributing to the Capital Framework](https://github.com/cfpb/capital-framework/#contributing),
which is the front-end pattern library used in this project.


----

## Open source licensing info
1. [TERMS](TERMS.md)
2. [LICENSE](LICENSE)
3. [CFPB Source Code Policy](https://github.com/cfpb/source-code-policy/)
