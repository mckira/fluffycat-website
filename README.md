# FluffyCat Website

## Development

### MacOS

* need to have [Jekyll](https://jekyllrb.com/) installed:

```bash
gem install jekyll bundler
```

* clone the repo
* because we are using some additional goodies, need to install them:

```bash
bundle install
```

* on my machine it was complaining about incompatible version of Ruby, need to install [RVM](https://rvm.io/rvm/install):

```bash
curl -sSL https://get.rvm.io | bash
rvm install 2.4.2
rvn use 2.4.2
```

* on my machine it was failing, apparently need to install Xcode command line tools:

```bash
xcode-select --install
```

* now you are ready and set up:

```bash
jekyll serve
```

* If you have issues with the command above, try the following:

```bash
bundle exec jekyll serve
```

## Domain Redirects

| Type          | Host          | Value                      |
| ------------- |:-------------:| --------------------------:|
| A Record      | @             | 192.30.252.153             |
| A Record      | @             | 192.30.252.154             |
| CNAME Record  | www           | fluffycatware.github.io.   |
| URL Redirect  | join          | http://fluffycat.tech/join |
| URL Redirect  | slack         | <custom join url>          |

## Technologies

* Created from ```jekyll new```
* added Netlify CMS in /admin/
* added Bootstrap 4 via CDN

## Attribution

This site is a baseline for an idea I have around donations to animal rescue. I used [Giveth's website](https://github.com/Giveth/website) as a foundation to get started