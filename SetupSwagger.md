# Setup Swagger to make API document


### Step 1 ###
Install library by Nuget
```
Install-Package Swashbuckle.AspNetCore -Version 6.2.3
```

### Step 2 ###
Register Service in Startup.cs
```
services.AddSwaggerGen();
```

### Step 3 ###
Setup Swagger middleware in Startup.cs
```
  app.UseSwagger();
  app.UseSwaggerUI(c =>
  {
      c.SwaggerEndpoint("/swagger/v1/swagger.json", "API List");
  });
```

### Step 4 ###
Open list api under path
```
https://localhost:7180/swagger/index.html
```
