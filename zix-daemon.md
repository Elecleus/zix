# zix-daemon

## Overview
zix-daemon is a background service that receives job requests from the zix CLI.

## Responsibilities
- Receive JSON payloads containing job information from zix CLI
- Execute corresponding actions based on the job specifications

## Features

### Build Process
1. Mount OverlayFS
2. Execute `pivot_chroot` into the new root environment
3. Perform build actions as specified

### Environment Access
1. Mount OverlayFS  
2. Execute `pivot_chroot` into the new root environment
3. Set up and enter the development environment