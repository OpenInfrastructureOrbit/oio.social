[![Build Status](https://travis-ci.org/OpenInfrastructureOrbit/oio.social.svg?branch=master)](https://travis-ci.org/OpenInfrastructureOrbit/oio.social)

Open Infrastructure Orbit
===========================
![#OIO - Open Infrastructure Orbit](https://oio.social/images/OIO-badge.svg "OIO")

This is the Website from the [Open Infrastructore Orbit](https://oio.social) - **OIO**.

Please feel free to create a Pull-Request.


 JEKYLL
---------

This website is generated with Jenkyll.<br/>
You can find more information about what jekyll is and how you can use it at [jekyllrb.com/docs](https://jekyllrb.com/docs/).

How to i18n
-----------

Every collections except posts (news, assemblies, pages) has language specific subfolders, where you can put your content. Blog posts have to be handled in another way: They have to be saved in a structure like `<language>/_posts` on the top level.

It's important, that for every content we have to set a `lang` tag, so it appears on the correct language specific overview pages (and will be linked). If the same content exists in both languages, we switch languages, if we also set a `ref` tag for the content.

How to run it locally
------------

**Kurzfassung:**
```bash
git pull
gem install jekyll bundler
bundle exec jekyll serve
```
