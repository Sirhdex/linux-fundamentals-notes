## Concepts
- Upkeep of our penetration distribution is important; we accomplish this through package management
- Many different files = many different package management systems
- The package management systems will retrieve the corressponding packages-- then download and install
- apt able to group .deb files, allowing us have no concern over distributions issues arising

## Commands
- dpkg -- install / manage Debian packages
- apt -- provides CLI for package management
- apptitude -- alternative to apt
- snap -- install / configure / refresh snap packages
- gem -- package management for Ruby; front-end for RubyGem
- pip -- python package managemen
- git -- fast, scalable, distributed control system; download tools from github
- apt-cache -- used to provide installed package information when offline
- wget (dpkg) -- download tools directly from repository 

## Examples
- apt-cache search [impacket]
- apt-cache show [impacket-scripts] -- view additional information about specific packet
- apt --list -- lists all installed packages
- sudo apt install impacket-scripts -y -- install package

