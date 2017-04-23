
# cliutils Library

## Introduction

The cliutils repository contains a small collections of command line utilities for unix like OSes (linux, darwin).

The goal is to share small tidbits for which I didn't find an obvious answer on the internet.

The programs are very small and, by design, use minimum dependencies so they can be used on a large number of systems.

Why perl? perl is installed by default on linux and darwin and has a lot of built in commands (minimum external dependencies). It is ideal to call other command line programs and parse their output.

Documentation: all scripts can be called without arguments or with '-h' or '--help' to get more information.

## Commands

### icmplookup

This script converts a hostname to an IP address using ICMP+DNS rather than DNS only. This is useful for the .local hostnames, when multicast DNS lookup is not setup. You would use this script when "nslookup <hostname>.local" fails on you LAN but you can still find the machine when using commands such as ssh or ping,

