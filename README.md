# Dockhand stack

This repository contains the standalone Dockhand Compose stack. Dockhand is
an operator tool for managing Docker workloads and is not deployed on the
Lighthouse host. The stack expects the host Docker socket and persistent
`/var/lib/dockhand` storage, and exposes its service through the `x-caddy`
route in `compose.yaml`.

Start it with a Docker Compose implementation that supports the repository's
`x-caddy` extension, or adapt that route to the ingress used by your host.

