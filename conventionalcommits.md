# Conventional Commits

## How to generate changelog based on conventional commit and git tags


Install the tooling ([source](https://github.com/conventional-changelog/conventional-changelog/tree/master/packages/conventional-changelog-cli))

```bash
npm install -g conventional-changelog-cli
```

Generate your very first changelog:

```bash
conventional-changelog -p conventionalcommits -i CHANGELOG.md -s -r 0 -t v
```

Update your changelog

```bash
conventional-changelog -p conventionalcommits -i CHANGELOG.md -s  -t v
```

> [how to config stuff / to be curated and tested](https://github.com/conventional-changelog/conventional-changelog/tree/master/packages/conventional-changelog-conventionalcommits)
