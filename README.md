Herd is a single-command Bittorrent-based file distribution system, based on Twitter's Murder.
It was designed for pushing code out to a number of production systems. You can probably use
it for other things.

Herd requires no extra Python modules on the destination system as it ships around
its own (lightly modified) copy of BitTornado.

## Usage

Herd assumes that you're running as a user which has passwordless SSH access,
with the same account, to all the machines you need to copy to.

Create a file hosts.dat with a list of the hosts you want to copy to, and:

    herd.py ./myfile.tar.gz /path/to/destination.tar.gz hosts.dat


-- Russ Garrett <russ@garrett.co.uk>
