## Add submodules
```
git submodule add git@github.com:wikip-co/public.git public/`
git submodule add git@github.com:wikip-co/wiki_theme themes/`
```

### Verify submodules
```
git submodule init
git submodule update
```

## Edit _config.yml
```
title: <Site Name>
subtitle: 'Documentation'
description: 'Research'
keywords:
author: <Author>
language: en
timezone: ''
url: https://wikip.co/<site-name>
root: /<site-name>/
permalink: :post_title/
permalink_defaults:
pretty_urls:
  trailing_index: true
  trailing_html: true
source_dir: source
public_dir: public/<site-name>
```

## Edit `resources.yml`
```
title: <Site Name>
cloudinary_user: <Cloudinary Username>
image_transform: /image/upload/w_200,f_auto/
image_cloud: https://res.cloudinary.com/
favicon: <favicon URL>
```

## How to Deploy

- Ensure submodules are up to date
- Generate static files, `hexo generate`
- Push changes to public submodule
- Push changes to source repo
