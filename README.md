# Fetch Golang Project!!

## Install and Run Instructions:
1 - Download Golang and install Go [HERE!](https://go.dev/doc/install)
2 - Once installed, make sure it works with `go version`
3 - While in the directory with the code, run `go mod init endpointchecker`, That will create a module of the go code for you.
4 - Then run `go mod tidy` to pull down the modules needed to run the code.
5 - Once all that is run, you are able to run the code with `go run main.go endpoint.yaml`. sample.yaml being the input for your code. You should see your endpoints after that!

### Fixed issues:
- yaml.v3 package was missing for the run, just downloaded it to fix 
- io/util was deprecated, fixed by removing since OS handles most of it. in the function at bottom, adjusted the readfile that was using it to the OS syntax



### Optimizations:
- [ ] Removed the io/util, one less mod to deal with when OS can handle it.
- [ ]  
