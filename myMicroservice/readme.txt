Dotnet CLI
------------------------------------------------------
------------------------------------------------------
Create a .NET Core API project
>dotnet new webapi -o myMicroservice --no-https
-o flag: create a folder for app.
--no-https flag: app runs without https certificate.

Run app
>dotnet watch run (in debug mode)
>dotnet run

------------------------------------------------------
------------------------------------------------------
Docker CLI
------------------------------------------------------
------------------------------------------------------
Check docker version on machine
>docker --version

Check docker images on machine
>docker images

Create docker image
>docker build -t <imagename> <folderpath to Dockerfile>
e.g.
>docker build -t mymicroservice .
Here . represents current folder.

Run app in docker container
>docker run -it --rm -p 3000:80 --name <containername> <imagename>
e.g.
>docker run -it --rm -p 3000:80 --name mymicroservicecontainer mymicroservice
Now test the app at http://localhost:3000

------------------------------------------------------
------------------------------------------------------
Git CLI
------------------------------------------------------
------------------------------------------------------
To check the status of files which are added/modified/deleted
>git status

To stage the changes for commit
>git add .

To commit the changes
>git commit -m "commit message here"

To push the changes to Github repository
>git push








