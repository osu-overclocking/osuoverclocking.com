
# OSU Overclocking Club Website

This is the website for the osu overclocking club.


## Installation

### Prerequisites

[Read the HUGO quick start guide](https://gohugo.io/getting-started/quick-start/)

You can check that Hugo is installed in the terminal by running:

```bash
hugo version
```

### Setup

Once the Hugo is installed, [clone the repository](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) to your local machine.

From the command line:

```bash
git clone git@github.com:osu-overclocking/osuoverclocking.com.git ./osuoverclocking.com
```

Finally, install the submodules to load themes.

```bash
git submodule update --init --recursive
```

### Local Development

You can run the server locally with drafts or not.

```bash
# No drafts
hugo server

# Drafts
hugo server -D
```

When Hugo is done building, you should see a success message like:

```bash
Web Server is available at //localhost:1313/ (bind address 127.0.0.1)
Press Ctrl+C to stop
```

## Contributing

Pull requests are welcome; although this site mostly for club leadership to write
posts and give information vital to the club. Check out our
[wiki](https://wiki.osuoverclocking.com)! as it is more accessible to outside contributions.

For more information about how this theme works, see the [ananke](https://github.com/theNewDynamic/gohugo-theme-ananke) repository.


### Posts

All posts are written in [markdown](https://www.markdownguide.org/basic-syntax/)!
You can use that to make fancy headings and other markings on the page.

To create a post, run

```
hugo new content post/{Post_Name}.md
```

which will create the template file.

> Note: You should use snake case for file names eg everything lowercase and underscores instead of spaces.

It should look similar to:

```
+++
title = 'Post_Name'
date = 2024-02-23T00:05:31Z
draft = true
+++
```

You can change the title there to make it more human readable. The draft section
controls whether the post is published or not; make sure to change that to true
when it is ready to be made public.

After that header, you can write markdown and it should be interpreted on the site.

### Submitting PRs

When you are ready for your changes to go live, submit a pr to the main repository
with your branch and it will be reviewed and be added to the repository.

## Partners

IEEE
OSU
MICRON
INTEL
ASUS
ELMOR LABS
TEKTRONIX

