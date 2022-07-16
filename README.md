# graphql-codegen-starter

This is a simple starter to set up a graphql-codegen project in the following way:

- it uses graphql-config to write a consistent configuration for various graphql based tools
- it creates an introspection of the graphql endpoint to allow developers to write valid queries without needing it always up
  - this also has the added benefits of working even for schemas that for any reasons extends graphql with custom directives
- it reads queries from graphql files put in the queries folder
- it generates schema and operations types in typescript
- it generates bindings for both react and vue via urql
- it uses eslint and prettier to lint and format your graphql files

## Usage

### Commands

This starter is configured to work with the following commands:

- `introspection` run it to update the schema introspection
- `codegen` run it to generate typescript files from your graphql files
- `lint` run it to lint your graphql files with eslint
- `format` run it to format your graphql files with prettier

### Demo

For demo purposes I already generated an introspection of Uniswap v3 subgraph and put a simple query to try it.


## Customizing

This is a simple starter that I tried to keep as generic as possible, you can obviously change stuff like using Apollo instead of Urql, just go to the graphql-codegen plugins page and look at what is available :).

