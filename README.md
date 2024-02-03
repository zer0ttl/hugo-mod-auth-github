# hugo-mod-auth-github

hugo-mod-auth-github is a Hugo module that integrates authentication via Github for you to use in your Hugo projects.

This module currently supports deployment only on Cloudflare Pages.

The files get mounted in `functions/api`.


## Requirements

- DecapCMS

You need to have DecapCMS already installed. You can follow the official tutorial to integrate DecapCMS into your Hugo project.

Alternatively, you could integrate hugo-mod-decapcms module in your Hugo project.

- Cloudflare account

## Use

1. Import the module into your Hugo project's site config as follows:

- Toml

```toml
[[module.imports]]
path = "github.com/zer0ttl/hugo-mod-auth-github"
```

- YAML

```yaml
module:
  imports:
    - path: "github.com/zer0ttl/hugo-mod-auth-github"
```

2. You can then add your own `static/admin/config.yml` file to modify the config for `backend`.

```yaml
backend:
  name: github
  repo: zer0ttl/test-netlifycms-cf-pages # Repo for your Hugo project
  branch: main # Branch to update (optional; defaults to master)
  base_url: https://test-netlifycms-cf-pages.pages.dev # Base URL to accept callbacks from Github
  auth_endpoint: /api/auth # Auth endpoint
```

3. Create an oauth app in Github

- [ ] #task #todo Add steps and screenshots.

4. Deploy to Cloudflare Pages.

- [ ] #task #todo Add steps and screenshots. 
