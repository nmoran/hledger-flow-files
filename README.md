# hledger-flow-files
Repository to hold useful rules files and preprocessing scripts for use with hledger-flow

All files are under the `my-finances` folder. To use with hledger-flow run

```
hledger-flow import ./my-finances/
```

which will create journal files from the `sample.csv` files. It is important to include the `./` or otherwise
hledger will fail to follow included journal files.

To use the generated journal files, can run hledger using journal file at `./my-finances/all-years.journal`. e.g.

```
hledger -f my-finances/all-years.journal
```
