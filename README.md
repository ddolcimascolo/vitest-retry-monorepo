# vitest-retry-monorepo

To reproduce: 
* Clone this repo
* Install dependencies using `npm i`
* Run tests in a single package folder using `--retry 2` option, and observe Vitest retrying twice

```
npm -C packages/package-1 test -- --retry 2
```

* Run tests at the root of the monorepo using `--retry 2` option, and observe Vitest **not** retrying

```
npm test -- --retry 2
```
