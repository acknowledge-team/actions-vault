# Acknowledge Github Actions for vault

## Purpose

This github actions can be called in your workflow to : 
* Download vault
* Install it in the PATH

## Usage

```
name: "Using Acknowledge vault action"

on: push

jobs:
  setup:
    name: "Setup vault"
    runs-on: self-hosted
    steps:
      - name: "Download and install"
        uses: acknowledge-team/actions-vault@main
        with:
          vault_version: "1.6.3"
```
