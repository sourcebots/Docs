---
title: Editor support
---

Installing our code locally will allow your editor to extract information from our code, giving you additional features like auto-complete (also known as [IntelliSense](https://en.wikipedia.org/wiki/IntelliSense)).

Installing these definitions is optional, but will be incredibly useful if your editor supports this. All editors in our [recommended list](/tutorials/editors/) besides IDLE will support it.

## Installation
Our API, the code you interact with, can be installed using Python's built-in package manager `pip`. On Windows, `pip` is already installed as part of Python; on other systems you'll need to look up how to install it. See [here](https://stackoverflow.com/a/12476379) for troubleshooting on Windows.

```bash
pip install git+https://github.com/sourcebots/robot-api
```

Simply start/restart your editor of choice, and it should detect our code and be able to autocomplete immediately.

## Upgrading installation

When we release new updates, you'll need to update the locally installed version too, so you have the most up to date definitions. To do this, simply repeat the previous command with `--update`:

```bash
pip install git+https://github.com/sourcebots/robot-api --update
```

## Permission error
The above commands may require administrator access to the computer. If you're getting a _Permission Denied_ error of some sorts, you may need to add `--user` to the end. This is likely needed on a shared computer, such as those you may find in your colleges.

```bash
pip install git+https://github.com/sourcebots/robot-api --user
pip install git+https://github.com/sourcebots/robot-api --update --user
```

{{% notice note %}}
On macOS / Linux, you could also use `sudo` to run the command as root. On Windows, you may need to re-run using [command prompt as an administrator](https://technet.microsoft.com/en-us/library/cc947813.aspx).
{{% /notice %}}
