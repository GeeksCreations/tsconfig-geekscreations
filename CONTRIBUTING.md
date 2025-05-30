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

## Building

After applying the changesets, run the following to make sure everything is up to date and working:
```sh
npm install
```

## Committing

Once the build completes successfully, you can commit the changes.

## Releasing

Releases are handled automatically via CI when a new Git tag is pushed. In order to create a tag run:

```sh
git tag vX.Y.Z
git push --tag
```