# psql-helpers

A small collection of helper functions to generate postgresql queries

# Examples

## Insert

```haskell
{-# LANGUAGE OverloadedStrings #-}
import           Database.PostgreSQL.Simple
import           Database.PostgreSQL.Simple.ToField

foo :: Connection -> IO ()
foo conn = insert "foo_table" ["bar" @= 5, "baz" @= True]
```
