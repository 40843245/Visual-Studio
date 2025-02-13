# How to add .edmx file in Visual Studio?
1. In solution explorer tab, select `<your-project>` -> `Models` directory.

where 

`<your-project>` is your project that you want (`.edmx` file will be built under this directory).

![image](https://github.com/user-attachments/assets/fe3633dc-2450-4324-83d9-4a4a533ef39a)

2. right click on that directory, then select `add`-> `add new item`
   
<img width="515" alt="image" src="https://github.com/user-attachments/assets/66e35508-8bd9-4765-b2f6-3ea374df8db3" />

3. select ADO.NET entity data model (in `Visual C#` -> `Web` -> `Data`)

and fill your name then click `Next`.

Shown as follows.

> [!CAUTION]
> recheck the name (for `.edmx` file), since it does not make any sense to rename it after it is created.

![image](https://github.com/user-attachments/assets/c52e35fb-204e-4b8c-b6ff-07aca61ce214)

4. select `EF designer from database`.

then click `Next`

Shown as follows.

![image](https://github.com/user-attachments/assets/1b4979fe-bc96-4998-8e21-cebd26e6b940)

5. select the data source from drop-down list

and determine to contain sensitive data in [connection string](https://learn.microsoft.com/en-us/aspnet/mvc/overview/getting-started/introduction/creating-a-connection-string) (type is radio button group).

untick the checkbox (將Web.Config中的連接設定儲存為)

then click `Next`.

![image](https://github.com/user-attachments/assets/c6983bdd-f35f-4c67-9481-5b6a320c246a)

