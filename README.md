# VInspect releases

**VInspect 1.0.0** is the first official Linux release for visual inspection of
KM3NeT DOMs, detection units, production batches and electronic components.

Developed by **Emiliano Librizzi** · **INFN Naples** · **Capacity Laboratory** · **KM3NeT**.

## Download and start

Download [**VInspect-Linux.tar.gz**](https://github.com/emilianolibrizzi/vinspect-releases/releases/latest/download/VInspect-Linux.tar.gz)
and its [SHA-256 checksum](https://github.com/emilianolibrizzi/vinspect-releases/releases/latest/download/VInspect-Linux.tar.gz.sha256).
Extract the complete archive into a new, empty folder such as **VInspect** and read
**START-HERE.md**. The executable and documents are directly inside it, with no
extra enclosing folder. Open **VInspect** to start the guided setup. Choose a language,
then **Install** into a new folder (default **~/VInspect**) with an optional Applications
menu shortcut, or choose **Use portable** to keep working in the extracted folder.
Python is included; no administrator privileges or system-wide installation are required.
The same compact archive supports both choices; there is no separate installer download.

Setup verifies the package before copying it and keeps existing archives untouched.
It creates a fresh installation and does not migrate site data. Existing installations
continue to open normally. **Menu → About → Create app shortcut** is also available
for portable use; keep the extracted folder in its chosen location.

The server supports **Linux x86-64 with glibc 2.34 or newer**, X11 or XWayland, and
the desktop libraries listed in the installation guide. Phones, tablets, Windows
and macOS computers connect through a browser. Each site runs its own server and
keeps its own inspection archive. This repository does not host laboratory data.

## Site activation

The server manager opens before activation. After reviewing and accepting the
licence, open **Menu → Settings → Sign-in → Site license**, copy the **Site ID**
and request an activation for your site from
[Emiliano Librizzi](mailto:emiliano.librizzi@gmail.com). Import the supplied signed
activation before starting the inspection server. Public download availability
does not grant unrestricted use or activate a site automatically.

Local password access works without Google or a cloud connection. Browser approval
can be enabled by the local administrator. Optional Google account access and
Drive copies require the site's own setup and the approvals described in the guides.
Trust the site's HTTPS certificate on client devices before using cameras or downloads.

## Inspection workflows

- DOM Integration and DU Integration projects with V1/V2 inspection profiles,
  English Excel exports, photographs, section progress and PMT observations.
- **Components Inspection** for Incoming electronic components: UPI/family
  identification, continuous photography, crop controls, recoverable browser queues,
  saved-photo archives and photographic PDFs. This workflow has no DOM report.
- Operator activity, planned work, takeovers and comparison with reviewed common
  edits across selected DOMs.
- Local project files and optional scheduled backups; personal Drive copies remain
  separate from the working archive.

The server manager and browser interface support English, Italian, French, German,
Dutch and Greek, with English as the default. Light, Dark and System appearance
are available. Official reports, documentation, diagnostic logs and the official
licence text remain English. Interface translation preserves identifiers and
user-entered inspection text.

## Signed updates and optional Site connection

The server manager checks the **Official** GitHub update source and verifies
Ed25519 signatures, file size and SHA-256 before installation. Checking or
downloading does not install anything. Stop the inspection server before choosing
**Install & restart**. Preserve the complete **VInspect_Data** or legacy **data**
folder and any custom storage locations when replacing an installation manually.

The separate versioned executable and
[`latest.json`](https://github.com/emilianolibrizzi/vinspect-releases/releases/latest/download/latest.json)
support the updater; they are not other application editions. The full archive is
the recommended first download. GitHub's automatic source archives contain this
repository's documentation, not VInspect's application source.

**Menu → Site connection** optionally connects one installation to the publisher's
private **VInspect Control** service using a site-specific connection file. It
reports the installation ID and application version and receives the assigned
signed-release policy. It does not give the site access to the publisher console,
other sites or remote desktop controls. Inspection databases, photographs, reports,
backups, operator lists and local passwords are not uploaded by this connection.
It does not configure Google sign-in, Drive, DNS or an Internet tunnel. An unavailable
control service pauses managed update delivery; ordinary local work continues
under the installed activation and access settings.

## Licence and attribution

This release includes the [**VInspect KM3NeT Use License 1.0**](LICENSE.VINSPECT.md),
effective **4 October 2026**. It permits fee-free authorised KM3NeT use and unchanged
compiled copies within that group, retaining attribution, the licence and third-party
notices. Other uses and modifications require written permission except where
mandatory law provides otherwise. The grant covers only rights the Licensor is
entitled to grant. Public availability does not make VInspect open source.

The operator accepts the exact bundled English terms before first operational use
and again if they change. Courtesy translations are available for consultation.
Reaching the end enables the acceptance checkbox, which must be selected explicitly.
Acceptance is stored locally and is not sent to the maintainer. Inspection data,
photographs and exported reports are outside the software licence's grant.

Licensing contact: **Emiliano Librizzi**, **Province of Caserta, Italy** —
[emiliano.librizzi@gmail.com](mailto:emiliano.librizzi@gmail.com).
The project affiliations provide context; they do not identify an institution as
Licensor or imply endorsement. Acceptance, attribution and release signatures do
not certify ownership or legal validity. The terms included with each copy apply
to that copy; matching version numbers do not change earlier copies retroactively.

## Verification and support

The full archive includes installation and workflow guides, licence notices,
verification records and checksums. Consult those records for the checks performed
on the supplied executable. Physical cameras, hotspot adapters, real Google/Drive
accounts, desktop appearance and sustained load still require checks at each site.
Use **Menu → View activity** and `./VInspect --check-runtime` for diagnostics.

Application source, site records, credentials, private signing keys and the private
administration service are excluded from this public release repository.
