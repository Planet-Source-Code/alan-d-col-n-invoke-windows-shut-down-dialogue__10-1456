<div align="center">

## Invoke Windows Shut Down Dialogue


</div>

### Description

This code causes the windows shut down dialogue to come up(see screenshot).
 
### More Info
 
Basically I came across the need to invoke this dialogue in my code. After a few hours of searching around the internet I found everyone was mostly calling "shutdown.exe" to get windows to shut down, but I wanted the dialogue you get when you click on start->shutdown in the start bar(see screenshot). As you can see I came up with a very very simple way of doing this. This isn't anything special but I thought someone else out there might wonder how to do this and I could save you some time by just posting this.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Alan D\. Colón](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/alan-d-col-n.md)
**Level**          |Beginner
**User Rating**    |4.7 (14 globes from 3 users)
**Compatibility**  |VB\.NET
**Category**       |[System Services/ Functions](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/system-services-functions__10-23.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/alan-d-col-n-invoke-windows-shut-down-dialogue__10-1456/archive/master.zip)





### Source Code

```
'Simply put this code anywhere in your project
'that you want the windows shut down dialogue box
'to be triggered.
'------------------------------------------------
Dim ExplorerProcess() As Process
ExplorerProcess = Process.GetProcessesByName("explorer")
ExplorerProcess(0).CloseMainWindow()
```

