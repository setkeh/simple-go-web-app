## Build the app
```
go build main.go
```
## Run the app
```
./main
```

or 

```
go run main.go
```

# Notes

* It looks like AWS does not support port redirect in CF yet and i could not find a way of doing this without haveing lambda or nginx proxy port 80 to 443.
* You will have to manually pre-link your github account to codebuild in the AWS Console buy creating a new codebuild project and going throught the OAUTH account linking steps for github, You can then cancel the project creation as it is not required as the CF will create it.