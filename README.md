Maritime Interfaces | ROS Messages
---
# Introduction
There is a need to create a standard interface for AUV, ASV's and USV's using ROS modules and drivers. There are some notable interfaces that are well maintained or sensible to utilize - as such this repository will use these modules and aggregate them into a single ros-installable `maritime-interfaces`.

# Scope / Goals
The intention of this repository is:
1. Provide a single source of interfaces for all AUV and ASV operations in ROS
2. Utilize existing interfaces to best provide ongoing maintenance
3. Allow for easy install / dependency by packaging as a `ros-<distro>-maritime-interfaces` package.
4. Maintained by repository contributors and organizations with their respective submodules

# Docs
Documentation will be found under [docs](.docs) in this repository. This will include the architecture, and detailed description of messages and their uses.

# Timeline
| Date    | Milestone                |
| ------- | ------------------------ |
| Aug, 22 | Architecture confirmed   |
| Nov, 22 | Draft Messages           |
| Dec, 22 | V1.0 maritime-interfaces |