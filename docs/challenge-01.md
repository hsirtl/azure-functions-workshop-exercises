# Challenge 1

## Create your first Azure Function (PowerShell)

1. Run the ```func init``` command, as follows, to create a functions project in a folder named LocalFunctionProj with the specified runtime:

    ```powershell
    func init LocalFunctionProj --worker-runtime powershell
    ```

1. Navigate into the project folder:

    ```powershell
    cd LocalFunctionProj
    ```

1. Add a function to your project by using the following command, where the --name argument is the unique name of your function (HttpExample) and the --template argument specifies the function's trigger (HTTP).

    ```powershell
    func new --name HttpExample --template "HTTP trigger"
    ```

### Load a sample template and make some edits 

1. Click on _Sample Template_.
1. Select the template ```microsoft.storage/storage-account-create/main.bicep```
1. Remove some ot the allowed values for ```storageAccountType``` and verify the effect on the compiled ARM template.
1. Optional: make further changes and verify their effect on the ARM template.