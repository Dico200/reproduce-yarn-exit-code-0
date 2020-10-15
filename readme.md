# Yarn run does not give correct exit code

## How to reproduce (windows)
- `yarn set version 2.3.3`
- `yarn run lint`
- `echo %errorlevel%`
- Notice the exit code is 0 despite errors
- `yarn set version 2.1.1`
- `yarn run lint`
- `echo %errorlevel%`
- Notice the exit code is (correctly) 1
