# Blazor Cookie Authentication

## Overview

This sample demonstrates how to implement cookie-based authentication in a Blazor Server application using ASP.NET Core authentication middleware. The project shows how authentication cookies are created, validated, and used to manage authenticated user sessions within a Blazor application.

The sample includes authentication configuration, cookie management through a dedicated controller, and Blazor pages that participate in the sign-in and authentication workflow. It is intended for developers who want to understand how cookie authentication can be integrated into a Blazor Server application without relying on external identity providers.

## Key Features

- Uses Blazor's `AuthorizeView` component to conditionally render content for authenticated users.
- Displays authenticated user information by retrieving the first available value from `context.User.Claims`.
- Demonstrates authentication-aware UI rendering through the `Authorized` content template.
- Shows how authenticated user claims can be accessed directly within a Razor component.
- Includes a simple HTML form for submitting a username to the server-side cookie authentication endpoint.
- Posts authentication data to the `cookie` endpoint using standard HTTP form submission.
- Demonstrates integration between Blazor pages and ASP.NET Core cookie-based authentication services.
- Provides a basic example of establishing and consuming authenticated user identities within a Blazor Server application.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download this repository.
2. Open `BlazorCookieAuthentication.sln`.
3. Restore the NuGet packages if prompted.
4. Build the solution.
5. Ensure the startup project is set to `BlazorCookieAuthentication`.
6. Press `Ctrl+F5` to run the application.

**Visual Studio Code**

1. Open the repository folder in Visual Studio Code.
2. Open a terminal and navigate to the project directory.
3. Restore the NuGet packages:

```bash
dotnet restore
```

4. Run the application:

```bash
dotnet run
```

5. Open the local application URL displayed in the terminal after startup.

## Project Structure

`Pages/Index.razor` - Main page that uses `AuthorizeView` to display authenticated user information and submits user credentials to the cookie authentication endpoint.

`CookieController.cs` - Handles cookie authentication operations, including processing form submissions and managing authentication cookies.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- For authentication implementation guidance, refer to the official ASP.NET Core Cookie Authentication documentation: https://learn.microsoft.com/en-us/aspnet/core/security/authentication/cookie?view=aspnetcore-10.0

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.