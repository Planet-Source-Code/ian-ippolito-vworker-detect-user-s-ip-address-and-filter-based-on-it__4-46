<div align="center">

## Detect User's IP address and filter based on it


</div>

### Description

If you have the need to filter out certain users from your site (hackers, unauthorized personel, etc.) and you know their IP address, you can use this code to do so. It detects the IP address of the current user and based on what that address is, takes action. Of course, you need to replace the IP address and the action in the code with whatever you would like to do...
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Ian Ippolito \(vWorker\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/ian-ippolito-vworker.md)
**Level**          |Beginner
**User Rating**    |4.8 (24 globes from 5 users)
**Compatibility**  |ASP \(Active Server Pages\)
**Category**       |[Server Side](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/server-side__4-31.md)
**World**          |[ASP / VbScript](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/asp-vbscript.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/ian-ippolito-vworker-detect-user-s-ip-address-and-filter-based-on-it__4-46/archive/master.zip)





### Source Code

```
<%@ Language=VBScript %>
<%option explicit
'get user's ip address
dim strUserIpAddress
strUserIpAddress = Request.ServerVariables("REMOTE_ADDR")
'check if this
If strUserIpAddress = "14.10.0.1" then ' put your IP here
	Response.write "You've been banned from this site!"
Else
	Response.write "Welcome to the site!"
End If
%>
```

