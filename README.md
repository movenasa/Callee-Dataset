# Callee-Dataset

This repo provides a dataset for indirect call recognition.


## Contents

```
.
|-- README.md
|-- funcs                   # Assembly functions of collected indirect calls
|   |-- callee              # Functions of collected callees. Each file corresponds to a binary, and each line consists of {callee_offset | callee_function_insns}
|   `-- callsite            # Functions of collected callsites. Each file corresponds to a binary, and each line consists of {callsite_offset | callsite_function_insns}
`-- icall.release.csv       # Indirect calls with columns (callsite_offset, callee_offset, callsite_binary, callee_binary)
```

## Acknowledgement

The dataset is built upon the following benchmarks:

 * [SPEC CPU 2006](https://www.spec.org/cpu2006/)
 * [UniBench](https://github.com/unifuzz/unibench)

And with the following tool:

 * [ibresolver](https://github.com/Learner0x5a/ibresolver)


```
