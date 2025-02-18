# Glam

Glam is a theme for The Balance website put together by the wonderful FFXIV community

## Testing the theme locally

Make sure you have [hugo](https://gohugo.io/getting-started/installing/) installed, either drop `hugo.exe` in the root dir or add it to your PATH.

```sh
# Clone the repository
git clone https://github.com/The-Balance-FFXIV/glam.git

# Navigate into it
cd ./glam/

# Install project dependencies and dependencies. If you prefer to not edit PATH, you can install globally.
export PATH=$PATH:node_modules/.bin
yarn install

# Run the servers
yarn start:static

# Server starts by default on `localhost:1313`
```


## Using the editor locally

First run the static site server with `yarn start:static`, then run `yarn start:admin` and navigate to `http://localhost:1313/admin`.
Alternatively, `yarn start` will start both servers.

# The wiggly bits
This is some general documentation until we can clean it out.

## Adding an item to the footer

Currently, the configuration for the footer is under exampleSite/config.toml.

If you want to add a new column, add it here.

Updating an entry: add it as a folder into exampleSite/content/*. You'll need to 
add an ``_index.md`` that will then list out the parent for that item, and other information
that you want to associate with it.
