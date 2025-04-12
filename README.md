Test project for external login - google

**It produces this error**

An unhandled exception occurred while processing the request.
AuthenticationFailureException: OAuth token endpoint failure: redirect_uri_mismatch;Description=Bad Request
Unknown location
AuthenticationFailureException: An error was encountered while handling the remote login.
Microsoft.AspNetCore.Authentication.RemoteAuthenticationHandler<TOptions>.HandleRequestAsync()


**How to run it**

Replace **XXXXXX** with your own values in Program.cs
```
builder.Services.AddAuthentication().AddGoogle(options =>
{
    options.ClientId = "XXXXXX";
    options.ClientSecret = "XXXXXX";
})
```

It is running in docker using **docker-compose.yml** included in project
