# Patankar.jl

Patankar.jl is an exploration of the ideas presented in Patankar's CFD book[^1],
using the [DrWatson](https://juliadynamics.github.io/DrWatson.jl/stable/)
framework.

To (locally) reproduce this project, do the following:

1. Clone this repo;
2. Open a Julia console and do:
   ```
   julia> using Pkg
   julia> Pkg.add("DrWatson") # install globally, for using `quickactivate`
   julia> Pkg.activate("path/to/this/project")
   julia> Pkg.instantiate()
   ```

This will install all necessary packages for you to be able to run the scripts and
everything should work out of the box, including correctly finding local paths.

You may notice that most scripts start with the commands:

```julia
using DrWatson
@quickactivate "Patankar.jl"
```

which auto-activate the project and enable local path handling from DrWatson.

## References

[^1]: Patankar, S. V. Numerical heat transfer and fluid flow. [s.l]: Taylor & Francis, 1980.
