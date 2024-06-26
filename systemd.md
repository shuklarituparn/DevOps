# Systemd files

The init system is the most important process on the linux system with the PID 1. It manages all the services that run in the background on the linux system. A unit is nothing but a type of resource that systemd can manage for us.

1. `/etc/systemd/system`: This directory contains systemd unit files created or customized by the system administrator to configure and manage system services, targets, sockets, devices, mounts, and timers.

2. `/run/systemd/system`: This directory stores runtime unit files generated by systemd during system boot or runtime modifications, typically for transient services or units created dynamically during system operation.

3. `/lib/systemd/system`: This directory holds the base set of systemd unit files provided by the system distribution, serving as a repository of default configurations for system services, targets, sockets, devices, mounts, and timers.

## Important Units

1. Service Units: Configure system services and daemons, specifying their lifecycle management, dependencies, and execution parameters.
2. Socket Units: Define inter-process communication endpoints for services, enabling communication over networks or locally.
3. Target Units: Represent system states or operational modes, providing synchronization points for starting or stopping multiple services simultaneously.
4. Path Units: Monitor files or directories for changes and trigger actions based on filesystem events, facilitating file-based activation of services.
5. Timer Units: Schedule periodic or one-time execution of tasks or services at predefined intervals or specific times.
6. Mount Units: Define file system mount points and their configuration, including options such as filesystem type and mount options.
7. Automount Units: Automatically mount filesystems on demand when accessed and unmount them when idle, improving system efficiency.
8. Device Units: Manage system devices and their configuration, providing control over device-specific settings and access permissions.
9. Scope Units: Organize system processes into hierarchical groups for resource management and control, particularly useful for managing transient tasks.
10. Slice Units: Organize system processes into hierarchical groups with resource allocation and control capabilities, enhancing system performance and stability.
