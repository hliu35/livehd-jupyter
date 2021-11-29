# Steps to create a GraphViz file (.dot)

### **Using `lgshell` to create LGraph files in (default) lgdb/**
```bash
livehd> inou.yosys.tolg files:./inou/yosys/tests/simple_add.v
```

### **To read LGraph files generated in lgdb/**
`simple_add.v` has no hierachy, so using `graphviz.from` not `graphviz.fromlg.hierachy`
```bash
livehd> lgraph.open name:simple_add |> inou.graphviz.from
livehd> exit
```
Now the file is saved to `simple_add.dot`

### **To visualize .dot files easily in VS Code**
Open .dot file with VS Code and use GraphViz extension to visualize




