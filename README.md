# Fetch Golang Project!!

## Install and Run Instructions:
1. Download Golang and install Go [HERE!](https://go.dev/doc/install)
2. Once installed, make sure it works with `go version`
3. While in the directory with the code, run `go mod init endpointchecker`, That will create a module of the go code for you.
4. Then run `go mod tidy` to pull down the modules needed to run the code.
5. Once all that is run, you are able to run the code with `go run main.go endpoint.yaml`. sample.yaml being the input for your code. You should see your endpoints after that!

### Fixed issues:
- yaml.v3 package was missing for the run, just downloaded it to fix 
- io/util was deprecated, fixed by removing since OS handles most of it. in the function at bottom, adjusted the readfile that was using it to the OS syntax



### Optimizations:
- [ ] Removed the io/util, one less mod to deal with when OS can handle it.
- [ ]  Added a GHA pipeline that runs the code for us. can be a cron somewhere but used it for this. Could also have the pipeline email the results in the health.txt but didnt wanna overdue to much. just show concept. Also i have it as a workflow manual so it isnt running all the time but added in code for the cron if i wanted to run on its own -- Yes I am embaressed at some of the small mistakes I made, feel free to make fun for syntax I got stuck on etc, I am doing this at 11ish pm for the pipeline portion so i am tired!
