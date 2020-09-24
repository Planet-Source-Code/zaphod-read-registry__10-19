<div align="center">

## Read Registry


</div>

### Description

Shows how to Read from the Registry using VB.net
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Zaphod](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/zaphod.md)
**Level**          |Intermediate
**User Rating**    |3.8 (19 globes from 5 users)
**Compatibility**  |VB\.NET
**Category**       |[Data Structures](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/data-structures__10-8.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/zaphod-read-registry__10-19/archive/master.zip)





### Source Code

```
Dim objKey As RegistryKey
 objKey = Registry.LocalMachine.OpenSubKey _
 ("SYSTEM\CurrentControlSet\Control\ComputerName _
 \ComputerName" , False)
 MsgBox(Convert.ToString(objKey.GetValue _
    ("ComputerName", "")))
```

