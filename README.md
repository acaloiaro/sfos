# SFOS 

Self-host OS.

The goal of this project is a fully-declarative self-hosting platform based on NixOS.

This is not an _actual_ operating system, but a collection of tools and Nix modules, built on top of NixOS, for 
bootstrapping and maintaining self-hosted platforms. 

Everything here is currently a work-in-progress.


## Bootstrapping the base system(s)

Considering [microvm](https://github.com/astro/microvm.nix/) as the primary bootstrap target for now.

[TBD](#TBD)

## Networking 

All networking is done with Headscale/tailscale internally, simplifying the interconnection of services.

## Virtualization and Containers 

[TBD](#TBD)

## Secrets 

There are two types of SFOS secrets.

1. Base system secrets which use [agenix](https://github.com/ryantm/agenix). These are used to bootstrap and manage the underlying infrastructure running SFOS.
2. Workload secrets, which use [setec](https://github.com/tailscale/setec) 
