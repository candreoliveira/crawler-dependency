# How to run a dependency script

Use the **npm explore** command. See more [here](https://www.arnaupujol.com/how-to-run-a-package-json-script-from-a-node-modules-dependency-with-npm-and-yarn/)

## Caution

All parameters you pass to the run script consider the submodule folder as working directory (CWD). Therefore, return to the root folder in the argument or pass the full path argument. For example:

If you want to use this root module **config.json** file, run the start script of crawl module as:

```
npm run start -- --file ../../../config.json --log debug --website magalu --page item -c 1 --type headless --admin
```

The **../../../** returns to the root dir.
