# @pnpm/plugin-commands-store-inspecting

## 0.1.0

### Minor Changes

- 97b450e1f: New commands added for inspecting the store:

  - **pnpm cat-index**: Prints the index file of a specific package in the store. The package is specified by its name and version: `pnpm cat-index <pkg name>@<pkg version>`
  - **pnpm cat-file**: Prints the contents of a file based on the hash value stored in the index file. For example:
    ```
    pnpm cat-file sha512-mvavhfVcEREI7d8dfvfvIkuBLnx7+rrkHHnPi8mpEDUlNpY4CUY+CvJ5mrrLl18iQYo1odFwBV7z/cOypG7xxQ==
    ```
  - **pnpm find-hash**: Lists the packages that include the file with the specified hash. For example:
    ```
    pnpm find-hash sha512-mvavhfVcEREI7d8dfvfvIkuBLnx7+rrkHHnPi8mpEDUlNpY4CUY+CvJ5mrrLl18iQYo1odFwBV7z/cOypG7xxQ==
    ```
    This command is **experimental**. We might change how it behaves.

  Related issue: [#7413](https://github.com/pnpm/pnpm/issues/7413).

### Patch Changes

- Updated dependencies [4e71066dd]
- Updated dependencies [33313d2fd]
- Updated dependencies [4d34684f1]
  - @pnpm/config@20.3.0
  - @pnpm/store.cafs@2.0.11
  - @pnpm/lockfile-types@5.1.5
  - @pnpm/types@9.4.2
  - @pnpm/pick-registry-for-package@5.0.6
  - @pnpm/client@10.0.42
