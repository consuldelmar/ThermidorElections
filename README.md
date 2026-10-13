# CAHT Election Simulator

An election simulator for the Civic Assembly of [Higher Thermidor](https://www.nationstates.net/nation=higher_thermidor), a nation on NationStates. It counts multi-member districts by the Single Transferable Vote, and you can set it up for any country: your own parties, districts, regions and vote transfers.

[**Open the simulator**](https://consuldelmar.github.io/ThermidorElections/) · [**Read the guide on NationStates**](https://www.nationstates.net/page=dispatch/id=2795939)

!\[The simulator after a run, with a three-party coalition selected](docs/screenshot.png)

## What it does

* Counts every district by STV with a Droop quota, passing on surpluses and eliminating the weakest party until all seats are filled.
* Moves transferred votes by how close parties sit on a two-axis political compass, or by a transfer table you edit yourself.
* Uses vote shares exactly as set, or treats them as polls and draws results around them, with optional momentum trends.
* Runs one election or up to 1,000, showing the median parliament and how much each party's seats vary.
* Lets you build coalitions, see the ways to reach a majority, and share out ministerial posts.
* Shows the chamber as a hemicycle or Westminster benches, with district, regional and compass views.
* Exports the chamber as PNG or SVG and the results as CSV, and saves the whole setup as a JSON file.

The guide on NationStates explains every option in detail.

## Using it

Open the link above, or download `index.html` and open it in any modern browser. It's a single file with nothing to install. It needs an internet connection only for its fonts.

To start from a ready-made setup, download a file from [`examples/`](examples/) and open it with **Load Config** in the sidebar:

* `higher-thermidor.json` is the default model: 9 parties, 10 provinces, 52 districts and 300 seats.
* `example-republic.json` is a small fictional country with 6 parties, 4 regions and 101 seats, a simple base for building your own.

Keyboard shortcuts: **R** or **Enter** runs one election, **N** runs the batch, and **Esc** closes an editor without keeping its changes.

## Credits and license

Created by F. Puyó, Consuldelmar and JuliaCerezo.

The code is released under the [MIT License](LICENSE). The flag of Higher Thermidor and its default dataset belong to the authors' NationStates worldbuilding and are included as an example; if you publish your own version, please replace them with your country's.

