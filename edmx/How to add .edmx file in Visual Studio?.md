# How to add .edmx file in Visual Studio?
> [!CAUTION]
> If you expect that Entity Data Model Wizard connects data from external data source (for example, external database)
>
> You must connect the database successfully before follow these steps. Otherwise, you won't see the external source as an option in the drop-down list (stated in step 5)
>
> A wrong example that happen on me:
>
> I forgot to connect the database (through MSSM (which stands for Microsoft SQL Server Management)).
>
> <img width="277" alt="image" src="https://github.com/user-attachments/assets/a62a17ee-01b3-45b1-97f1-b944b20f120f" />
> 
> Then in step 5, the available option is
>
> ![image](https://github.com/user-attachments/assets/c6983bdd-f35f-4c67-9481-5b6a320c246a)
 

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

5. select the data from data source (such as external database) that Entity Data Model Wizard connects to (from drop-down list)

and determine to contain sensitive data in [connection string](https://learn.microsoft.com/en-us/aspnet/mvc/overview/getting-started/introduction/creating-a-connection-string) (from radio button group).

untick the checkbox (將Web.Config中的連接設定儲存為)

then click `Next`.

![image](https://github.com/user-attachments/assets/e524e0b0-14df-45d2-8e18-71d91480cf6c)

6. wait for a while.
7. restart the VS to make the change effect.

> [!WARNING]
> Since VS IDE does not support hot reloading, please save it and restart the VS to make the change effect. 

## demo
See [How to create .edmx file in VS IDE?](https://youtu.be/tpkRdFHZRBI)

## troubleshoot
### Entity Data Model Wizard in VS failed to connect database
see [Visual Studio Entity Data Wizard, Crashes when Trying to Connect to Oracle](https://stackoverflow.com/questions/50911394/visual-studio-entity-data-wizard-crashes-when-trying-to-connect-to-oracle)

see [entity-framework -- ADO.NET Entity Data Model error](https://learn.microsoft.com/en-us/answers/questions/807003/entity-framework-ado-net-entity-data-model-error)
