# Minimal Reproduction (npm i @clerk/remix fails for Remix V2)

## Context

This repo contains a fresh and untouched (apart from this README.md file) install of Remix V2, installed as follows 

```sh
npx create-remix@latest
```

## Minimal Reproduction steps

Step 1: attempt to install @clerk/remix

```sh
npm i @clerk@remix
```

## Expected behavior: 

@clerk/remix successfully installs


## Actual behavior:

@clerk/remix fails to install with the following error:

```
npm i @clerk/remix
npm ERR! code ERESOLVE
npm ERR! ERESOLVE unable to resolve dependency tree
npm ERR!
npm ERR! While resolving: clerkremixv2installissue@undefined
npm ERR! Found: @remix-run/react@2.0.0
npm ERR! node_modules/@remix-run/react
npm ERR!   @remix-run/react@"^2.0.0" from the root project
npm ERR!
npm ERR! Could not resolve dependency:
npm ERR! peer @remix-run/react@"^1.7.6" from @clerk/remix@2.10.2
npm ERR! node_modules/@clerk/remix
npm ERR!   @clerk/remix@"*" from the root project
npm ERR!
npm ERR! Fix the upstream dependency conflict, or retry
npm ERR! this command with --force or --legacy-peer-deps
npm ERR! to accept an incorrect (and potentially broken) dependency resolution.
```
