# Codemods

This repository contains a collection of codemods designed to automate migration and upgrade processes.

Codemods are a powerful tool to automate code transformations, reducing the time and effort required to keep projects up-to-date.

All the codemods in this repository are published on the [Codemod Registry](https://codemod.com/registry?author=akash-kumar-dev), a public registry for codemod scripts aimed at simplifying migration and upgrade tasks.

### Available Codemods

Currently, this repository includes the following codemod for migration:

- **Sentry.js v7.x to v8.x Migration**: A codemod to help automate the upgrade from Sentry.js v7.x to v8.x. The migration recipe can be used to execute all required transformations for the upgrade.

All published codemods can be found on the [Codemod Registry here](https://codemod.com/registry?author=akash-kumar-dev).

---

## How to Use

### Installation

To get started, install the `codemod` CLI globally by running the following command:

```bash
npm install -g codemod
```

### Running Codemods

After installing the `codemod` CLI, use it to apply a specific codemod transformation to a project. To run a codemod, the following command format is used:

```bash
npx codemod <codemod_name> --target <path_to_project> [additional_options]
```

- **<codemod_name>**: The name of the transformation (e.g., `sentry/v8/migration-recipe`).
- **<path_to_project>**: The directory or file path to apply the transformation. By default, it will target the current directory.

For example, to migrate from **Sentry.js v7.x to v8.x**, run the following:

```bash
npx codemod sentry/v8/migration-recipe
```

This command will apply all necessary codemods to upgrade the project to Sentry.js v8.x.

---

## Caution

It is important to **commit any unsaved changes** before running these codemods. Since these scripts modify source code, they should be used with caution. Always ensure version control is in place or backups are available to avoid potential issues during the migration process.

---


Contributions and feedback are always welcome. Feel free to open issues or contribute improvements as needed!

---
