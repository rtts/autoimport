We'd love you to contribute to *autoimport*!

## Issues

Questions, feature requests and bug reports are all welcome as issues.
**However, to report a security vulnerability, please see our [security
policy](https://github.com/lyz-code/autoimport/security/policy).**

To make it as simple as possible for us to help you, please include the output
of the following call in your issue:

```bash
python -c "import autoimport.version; print(autoimport.version.version_info())"
```

Please try to always include the above unless you're unable to install
*autoimport* or **know** it's not relevant to your question or feature
request.

## Pull Requests

It should be extremely simple to get started and create a Pull Request.
*autoimport* is released regularly so you should see your improvements
release in a matter of days or weeks.

!!! note
    Unless your change is trivial (typo, docs tweak etc.), please create an
    issue to discuss the change before creating a pull request.

If you're looking for something to get your teeth into, check out the ["help
wanted"](https://github.com/lyz-code/autoimport/issues?q=is%3Aopen+is%3Aissue+label%3A%22help+wanted%22)
label on github.

To make contributing as easy and fast as possible, you'll want to run tests and linting locally.

You'll need to have **python 3.6**, **3.7**, or **3.8**, **virtualenv**, **git**, and **make** installed.

```bash
# 1. clone your fork and cd into the repo directory
git clone git@github.com:<your username>/autoimport.git
cd autoimport

# 2. Set up a virtualenv for running tests
virtualenv -p `which python3.7` env
source env/bin/activate
# (or however you prefer to setup a python environment, 3.6 will work too)

# 3. Install autoimport , dependencies and configure the pre-commits
make install

# 4. Checkout a new branch and make your changes
git checkout -b my-new-feature-branch
# make your changes...

# 5. Fix formatting and imports
make format
# autoimport uses black to enforce formatting and isort to fix imports
# (https://github.com/ambv/black, https://github.com/timothycrosley/isort)

# 6. Run tests and linting
make
# there are a few sub-commands in Makefile like `test-code` or `test-examples`
# which you might want to use, but generally just `make` should be all you need

# 7. Build documentation
make docs
# if you have changed the documentation make sure it builds successfully
# once built it will serve the documentation at localhost:8000

# ... commit, push, and create your pull request
```

**tl;dr**: use `make format` to fix formatting, `make` to run tests and linting & `make docs`
to build the docs.