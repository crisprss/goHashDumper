# goHashDumper

## Note
Dump内存都需要管理员权限

## Description 
用于Dump指定进程的内存,主要利用静默退出机制(SilentProcessExit)和Windows API(MiniDumpW)实现

## Usage
```
gohashdumper.exe -method 1 -out test.dmp -process lsass.exe
gohashdumper.exe -method 2 -path C:\tmp -pid 2333
  -method string
        choose Dump file Method(1 => MiniDumpW  2=> SilentExitDump) (default "1")
  -out string
        dump file name (default "lsass.dmp")
  -path string
        only method 2 need a filepath (default "D:\\RedTeam\\GoHashDumper")
  -pid string
        If not use process name,it can support pid
  -process string
        Process to dump (default "lsass.exe")
 ```
 
 ## Example
 ![](https://github.com/crisprss/goHashDumper/blob/main/image.png)
