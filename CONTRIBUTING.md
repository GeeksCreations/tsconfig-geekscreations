# Contributing

## Creating a Changeset

For any change that requires a version bump, run:

```sh
npx changeset
```

Follow the prompts to describe the change and select the affected package(s).

## Applying Changesets

After one or more changesets have been created, run:

```sh
npm run version
```

This will:

- Apply the changesets

- Update the package.json version

- Generate/update the CHANGELOG.md file

## Releasing

Releases are handled automatically via CI when a new Git tag is pushed. Changeset generates the tag automatically, so make sure to push it:

```sh
git push --tag
```