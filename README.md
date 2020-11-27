# Golang Project using Glide

This project is an example of a Golang project using Glide as its package manager and with the dependencies' versions locked down with glide.lock

`glide.lock` at the root directory declares the dependencies:
- github.com/google/go-github (version 173908142398084e14d7f14c39924f0004d43679)
- github.com/google/go-querystring (version 53e6ce116135b80d037921a7fdd5138cf32d7a8a)
- github.com/square/go-jose (version 7f0dd807d3f3d73bb536898cb7980ddf638ce69a)

Total number of dependencies:
- 3 direct dependencies.
- 1 transitive dependency. `github.com/google/go-querystring` is a direct and also transitive dependency (of github.com/google/go-github).
- 3 vulnerabilities.

#### Vulnerable Call Chain
This project does not have a vulnerable call chain. If you would like to test this feature, feel free to create a vulnerable call chain by modifying `main.go` and send us a PR.

#### What's next?
By running the security scanner of your choice against `with-glide.lock` project, you should get results that are coherent with the details above if the tool supports scanning Golang projects using Glide as their package manager.
