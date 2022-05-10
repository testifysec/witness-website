---
title: "Environment"
linkTitle: "Environment"
date: 2022-05-01
description: "Collect information about the environment"
---

The Environment Attestor records the OS, hostname, username, and all environment variables set
by TestifySec Witness at execution time.  Currently there is no means to block specific environment variables
so take care to not leak secrets stored in environment variables.
