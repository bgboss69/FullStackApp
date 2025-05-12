# FullStackApp

## How to Clone and Test

### Step 1: Clone the Repository
1. Open a terminal or command prompt.
2. Run the following command to clone the repository:
   ```bash
   git clone [<repository-url>](https://github.com/bgboss69/FullStackApp.git)
   ```
   Replace `<repository-url>` with the actual URL of the FullStackApp repository.

3. Navigate to the cloned directory:
   ```bash
   cd FullStackApp
   ```

### Step 2: Start the Server
1. Navigate to the `ServerApp` directory:
   ```bash
   cd ServerApp
   ```
2. Run the server:
   ```bash
   dotnet run
   ```

### Step 3: Update the Client Configuration
1. Open the `ClientApp/Program.cs` file.
2. Locate the following code:
   ```csharp
   builder.Services.AddHttpClient("ServerAPI", client =>
   {
       client.BaseAddress = new Uri("http://localhost:5082");
   });
   ```
3. Replace `http://localhost:5082` with your server's actual address.

### Step 4: Start the Client
1. Open a new terminal or command prompt.
2. Navigate to the `ClientApp` directory:
   ```bash
   cd ClientApp
   ```
3. Run the client:
   ```bash
   dotnet run
   ```

### Step 5: Access the Application
1. Open a web browser.
2. Navigate to `client localhost address` to view the client application.

### Notes
- Ensure you have the .NET SDK installed on your machine.
- If you encounter any issues, check the logs in the terminal for error messages.

