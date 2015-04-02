how to find namespace to package match in aspnet 5.0 and above to be included in project.json file.
http://www.nuget.org/packages?q=SYstem.Math

//from project.json file:
"frameworks": {
        "aspnetcore50": {
            "dependencies": {
                "System.Console": "4.0.0-beta-22523",
                "System.Runtime.Extensions": "4.0.10-beta-22605" //(this package contains System.Math class. include this in dependencies to have System.Math identified within build
            }
        }
    }
