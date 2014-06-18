trinity-docker
==============

Dockerfile for Trinity kernel/syscall fuzzer

This image when run (run as non-root using '-u'),
will fuzz the kernel and, should there be a container-breakout
vulnerability, may possibly exploit it.

Using this tool, I've personally discovered at least one
breakout. One user even told me they managed to crash
the Qemu process that their Docker host was running inside.

Authors
=======
Eric Windisch <ewindisch@docker.com>
