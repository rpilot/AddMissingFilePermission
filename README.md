# AddMissingFilePermission
Take file ownership (if needed) and add missing NTFS permissions

Useful script for file migrations to cloud. Especially when working with directory structures where inheritance is broken and current user can't access the file to copy it to cloud storage.

Example:

AddNasuniAccess -path "someFile.txt" -identity "BUILTIN\Administrator" -logFile "errors.csv"

It is setting local Administrators group as owner of the file only when needed.
It then assigns FullControl control.
All errors are written to the file mentioned in the logFile parameter
