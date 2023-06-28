---
sidebar_position: 1
---

# Introduction

TrueCharts is a catalog of highly optimised TrueNAS SCALE Charts. Made for the community, By the community!

This manual contains general information on working with TrueCharts Charts.

:::tip

Please, always remember to check the content specific to the chart.

:::

# Concept

## Integration between applications

Original TrueNAS Charts are standalone applications that can be used independently.

In contrast Truecharts applications are designed to use "core" applications for simplicity and unification:
- `Traefik` is an `Ingress` / `Reverse-Proxy` that provides access to applications from outside TrueNAS.
- `CloudNativePG` (or `CNPG` for short) is a database solution.

There are also other applications that are recommended for certificate management, authentication, DNS, etc.

## Application storage

Truecharts applications are designed to store all information within containers. It's not recommended to use Host Path to store data.

If application uses database, then it usually starts `CloudeNativePG` in the application deployment. Database data is also stored within container.

## Backup and restore

`Heavyscript` is a bash script for managing Truenas SCALE applications, automatically update applications, backup applications datasets, open a shell for containers, and many other features.

# First installation

Please check [Getting Started with TrueCharts inside TrueNAS SCALE](https://truecharts.org/manual/SCALE/guides/getting-started) for more information.

:::tip

Don't forget to read [FAQ](https://truecharts.org/manual/FAQ) before use start using Truecharts applications. It contains important information.

:::
