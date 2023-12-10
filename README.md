Build this solution.
```cmd
dotnet build
```

```txt
Build started...
1>------ Build started: Project: ConsoleApp1, Configuration: Debug Any CPU ------
1>D:\SadPencil\Documents\GitHub\polyfill-index-range-issue\Program.cs(8,37,8,40): error CS0518: Predefined type 'System.Range' is not defined or imported
1>D:\SadPencil\Documents\GitHub\polyfill-index-range-issue\Program.cs(8,37,8,38): error CS0518: Predefined type 'System.Index' is not defined or imported
1>Done building project "ConsoleApp1.csproj" -- FAILED.
========== Build: 0 succeeded, 1 failed, 0 up-to-date, 0 skipped ==========
========== Build started at 20:57 and took 00.519 seconds ==========
```

Change `ConsoleApp1.csproj` file to test the difference.
```xml
    <!-- This is a workaround. Uncomment the next line to test the difference. -->
    <!-- <DefineConstants>$(DefineConstants);NET48X</DefineConstants> -->
```