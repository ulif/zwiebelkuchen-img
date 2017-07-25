# Differences

In building the `zwiebelkuchen` we follow (somewhat loosely) the Adafruit way
to build an Onion-PI. the differences from this build are described here.

Here we document the differences from the stock Raspbian build (part 1) and
from the Adafruit build (part 2) as described on the respective web pages. The
first part is not very extensive because the details are pretty much covered in
the Onion-PI documentation.


## Differences to Raspbian Litie (roughly)

- Missing build stages

  We support only the Raspbian lite image, i.e. we skip build steps 4+ from
  `pi-gen`.

- Additional packages

  We install some extra-packages:

  - `unattended-upgrades`


## Differences to Adafruit Onion-PI

- IPv4 forwarding is disabled.

- We use CCC and digitalcourage.de DNS servers instead of Google.

- Firewall rules are flattened in order to be more concise.

- `unattended-upgrades` are installed and activated to run every other hour.

- `rng-tools` are installed to make use of the builtin random number gnerator.


