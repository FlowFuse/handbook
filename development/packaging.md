Flow Forge Packaging Guidelines

## Github projects 

### Naming

- Flow Forge Components should start with `flowforge-`
- If a Node-RED plugin/node should start with `flowforge-nr-`
- Installers or Orchestration projects are named without the leading `flowforge-` e.g. `installer` or `helm`

### Content

All Git Repositories must contain the following files:

 - README.md
 - LICENSE

### Notifications

Repositories should be added to the appropriate Slack channel. For core code reposities,
this would be in the `#gh-flowforge` channel.

To create a subscription, go to that channel and type the message:

```
/github subscribe flowforge/NAME-OF-REPO comments
```

This will subscribe to any notifications covering: `issues`, `pulls`, `commits`, `releases`, `deployments` and `comments`

## NPM packages

### Naming

- All packages should be scoped to `@flowforge`

Node-RED plugins should start with `nr-` e.g. 
 - @flowforge/nr-storage
 - @flowforge/nr-auth

Flow Forge plugins should start with `forge-` e.g.

 - @flowforge/forge-driver-localfs
 - @flowforge/forge-driver-docker
 - @flowforge/forge-driver-k8s

### Content

The `package.json` must contain the following keys

 - description
 - repository
     ```
     "repository": {
        "type": "git",
        "url": "git+https://github.com/flowforge/flowforge.git"
    },
    ```
 - homepage
    ```
    "homepage": "https://github.com/flowforge/flowforge#readme",
    ```
 - bugs
    ```
    "bugs": {
        "url": "https://github.com/flowforge/flowforge/issues"
    },
    ```
 - license
   - Apache-2.0
   - SEE LICENSE IN ./LICENSE
 - author
    ```
    "author": {
        "name": "FlowFlow Inc."
    },
    ```
 
### Package Version Numbering

Package numbers should follow the Semantic Versioning Scheme as laid out on [semver.org](https://semver.org/).

Each component will maintain it's own numbering regardless of the core FlowForge project and only update it's version as needed.