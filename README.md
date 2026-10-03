# VInspect releases

Release downloads and signed software updates for **VInspect**, a visual inspection
application for KM3NeT DOMs, detection units and production batches.

Developed by **Emiliano Librizzi** · **INFN Naples** · **Capacity Laboratory** · **KM3NeT**.

## Downloads

Use the [Releases page](https://github.com/emilianolibrizzi/vinspect-releases/releases)
for the complete installation package, requirements and release notes.

For a first installation, download **VInspect-Linux.tar.gz**, extract it into a new
folder and open **VInspect** directly inside it. The archive has no extra enclosing folder. Read **START-HERE.md** in that folder for
setup instructions. The accompanying `.sha256` file provides the archive checksum.
The separate versioned executable and `latest.json` are used by the built-in
updater. Keep your existing inspection data when upgrading an installation.

The server application targets Linux x86-64. Operators on computers, tablets and
phones connect through a browser. Each laboratory runs its own server and manages
its own inspection archive; this repository does not host laboratory data.

The native server manager and browser interface offer English, Italian, French,
German, Dutch and Greek. English is the default. Report headings, diagnostic logs,
licence terms and official documentation remain in English; user-entered data is
preserved. Client language preferences survive software updates.

## Software updates

Compatible VInspect clients can use the **Official** update source in the server
manager. Release metadata is signed with Ed25519 and clients verify downloaded
executables before installation. Checking or downloading an update does not install
it automatically.

The official update manifest is
[`latest.json`](https://github.com/emilianolibrizzi/vinspect-releases/releases/latest/download/latest.json).
Earlier clients need a one-time manual installation of a build containing the
updater.

## Repository contents

This repository contains release documentation and compiled release assets.
Application source, inspection records, credentials and private signing keys are
not published here.

## Licence and attribution

Public releases from **1.0.0** expressly carrying
[LICENSE.VINSPECT.md](LICENSE.VINSPECT.md) use the **VInspect KM3NeT Use License 1.1**,
effective 3 October 2026. It permits fee-free use for authorised KM3NeT activities
and sharing unchanged compiled copies within the authorised group. Retain the
author attribution, licence and third-party notices supplied with each release.

Use outside that scope and software modifications require separate written
permission, except where mandatory law provides otherwise. The licence covers only
rights held by Emiliano Librizzi and does not restrict independent third-party
permissions. Public availability does not make VInspect open source or grant use
for unrelated activities. Inspection data, photographs and exported reports are
outside the software licence's grant.

The server operator reviews and accepts the full English terms on first launch,
and again only if those terms change. This local acknowledgement is not sent to
the maintainer and does not determine copyright ownership.

For licensing enquiries: **Emiliano Librizzi**, Naples, Italy —
[emiliano.librizzi@gmail.com](mailto:emiliano.librizzi@gmail.com).

Official documentation and release notes are in English. Author attribution records
the development contribution; it does not by itself determine ownership or imply
institutional endorsement.
