# NPM Service
> Based on Verdiccio

### Create User
* Before create user, you should set `max_users` not -1
  * edit `/configs/plugins/service/config/npm/config.yaml`

```
npm adduser --registry https://YOUR_NPM_REGISTRY_DOMAIN
```

### Login

```
npm login --registry https://YOUR_NPM_REGISTRY_DOMAIN
```

### FAQ
* Yarn Add : authorization required to access package
  * Solved:
    * CMD: npm config set always-auth true
    * .npmrc: //registry.your-private.org/:always-auth=true
  * Reference:
    * https://github.com/verdaccio/verdaccio/issues/1529


