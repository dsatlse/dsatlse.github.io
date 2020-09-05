# Website for the LSESU Data Science Society

This is a static [website](https://dsatlse.github.io/) made with [Zola](https://www.getzola.org/). All public materials developed by the society will be available on it, along with documentation of projects, events and public Zulip communication.

## Build

Install Zola as described [here](https://www.getzola.org/documentation/getting-started/installation/) or, and this is the easiest if you are used to the command line, download precompiled binaries for your platform from [here](https://github.com/getzola/zola/releases).

Run `zola build` in order to build and `zola serve` to run a small server. It will also reload automatically on changes made to the files. With the help of GitHub Actions this website is built automatically on each new commit. You can see the whole build process in `.github/workflows/main.yml`.

## Content

- Content i.e. materials, events, projects in `/content`
- Static files e.g. images in `/static`
- Templates which define the structure in `/templates`

The templates should be treated as part of the design and edited in last resort.

## Contribution

Below is the least amount of steps to get from a fresh Git installation to changing
content on this site. To be extended with detailed explanations.

Inform your Git about your identity as follows
```
git config --global user.name "Your name"
git config --global user.email "Your email"
```

Then clone this repository
```
git clone https://github.com/dsatlse/dsatlse.github.io.git
```

After making changes to your local state, assuming you have push rights, run the following
```
git add .
git commit -m "Add content on metric embedding"
git push
```


## Principles

This is an outline of the technical stack for the LSESU Data Science Society. Here's a bunch of principles. In one word we want to focus on continuity.

+ Requiring minimal IT competence to maintain
+ Clear documentation of the tools and how they relate to each other
+ Liberal enough to extend without reinventing the wheel
+ Easy transfer of ownership to subsequent committees
+ Ideally keep the core pieces stable on unpaid plans
+ Plug-and-play nature of components: if something is not used, don't force it

[@kowale 2020](github.com/kowale)
