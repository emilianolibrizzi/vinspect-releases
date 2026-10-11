# VInspect releases

**VInspect 1.0.0** is the first official Linux release for visual inspection of
KM3NeT DOMs, detection units, production batches and electronic components.

Developed by **Emiliano Librizzi** · **INFN Naples** · **Capacity Laboratory** · **KM3NeT**.

## Download and install

Download [**VInspect-Setup**](https://github.com/emilianolibrizzi/vinspect-releases/releases/latest/download/VInspect-Setup)
and its [SHA-256 checksum](https://github.com/emilianolibrizzi/vinspect-releases/releases/latest/download/VInspect-Setup.sha256).
This **single executable** contains the application, bundled Python, guides,
licence and third-party notices. Open it, choose your language and installation
folder (default **~/VInspect**), then **Install → Open VInspect**. The guided
installer includes progress and an optional Applications-menu shortcut.

Linux may require **Properties → Permissions → Allow executing file as program**
first. From a terminal in the download folder, use `chmod +x VInspect-Setup`, then
`./VInspect-Setup`. Do not use `sudo`. Setup needs no archive extraction, Python
installation or administrator privileges. It verifies the included files, creates
fresh storage and leaves existing archives untouched. It is not an archive
migration or in-place update tool. Its private temporary files are removed when
setup closes; the installed application and site data remain in the chosen folder.

For portable use, [**VInspect-Linux.tar.gz**](https://github.com/emilianolibrizzi/vinspect-releases/releases/latest/download/VInspect-Linux.tar.gz)
and its [checksum](https://github.com/emilianolibrizzi/vinspect-releases/releases/latest/download/VInspect-Linux.tar.gz.sha256)
remain available. Extract the complete archive into a new empty folder, open
**VInspect** and choose **Use portable**. **START-HERE.md** explains installation,
activation and migration. This is the same application, not a different edition.

The server supports **Linux x86-64 with glibc 2.34 or newer**, X11 or XWayland, and
the desktop libraries listed in the installation guide. Phones, tablets, Windows
and macOS computers connect through a browser. Each site runs its own server and
keeps its own inspection archive. This repository does not host laboratory data.

## Activate the site

After reviewing and accepting the licence, request a private activation code from
[Emiliano Librizzi](mailto:emiliano.librizzi@gmail.com), giving your laboratory's
name. Open **Menu → Settings → Sign-in → Site license** in the manager, paste the
code into **Activation code** and choose **Activate** while online. One step
obtains the signed licence, registers the site and connects its update controls.
No separate Site ID exchange or connection-file import is needed for this route.

A code normally expires after **24 hours** and activates one server computer.
The activation window opens during initial setup. **Resume activation** recovers an
interrupted exchange using the saved claim. The manager remains available without
activation; the inspection server requires a signed machine-bound licence and a
fresh online authorisation at every start. Multiple operator browsers may connect
to that server according to its local access policy.

Authorisation is renewed **every minute** and lasts at most **15 minutes**. Brief
Internet interruptions are tolerated until expiry; then new protected work pauses
until verification succeeds. Existing files and recoverable browser drafts remain
intact. A replacement computer requires publisher-approved transfer, even if the
complete archive was copied. Older offline-only grants require online activation.
Public availability does not grant unrestricted use or activate a site.

Managed updates initially remain on **Hold** until the publisher assigns a release
policy. This does not prevent local inspection work. Local password access works
without Google; these local profiles require site and publisher approval. Google
account access and Drive copies require separate site configuration and approvals.
Trust the site's HTTPS certificate on client devices before cameras or downloads.

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

## Signed updates and Site connection

The server manager checks the **Official** GitHub update source and verifies
Ed25519 signatures, file size and SHA-256 before installation. Checking or
downloading does not install anything. Stop the inspection server before choosing
**Install & restart**. Preserve the complete **VInspect_Data** or legacy **data**
folder and any custom storage locations when replacing an installation manually.

The separate versioned executable and
[`latest.json`](https://github.com/emilianolibrizzi/vinspect-releases/releases/latest/download/latest.json)
support the updater; they are not other application editions. The full archive is
available for portable use; **VInspect-Setup** is the recommended first download. GitHub's automatic source archives contain this
repository's documentation, not VInspect's application source.

**Menu → Site connection** manages the credential created during activation.
The publisher's private **VInspect Control** service authorises the bound server
and supplies its site/group/global signed-release policy. Site clients have no
owner-console privileges, access to other sites or remote desktop controls.
The publisher controls the release source and signing key. Site managers choose
when to install, but cannot disable required checks or change that trust policy.

The service receives site/licence identifiers, a site-specific machine hash,
application versions and minimal session/contact metadata. Raw hardware identifiers,
inspection databases, photographs, reports, backups, passwords and Drive tokens
are not uploaded. Google sign-in ID tokens are transmitted over HTTPS for independent
central verification and are not stored or logged. A limited operator roster (names, verified emails when present,
identity category, approval and activity status) supports publisher access control. This connection does not configure Google sign-in,
Drive, DNS or an Internet tunnel. A revocation reaches a connected server at its
next check; a disconnected server can retain authorisation until it expires.

These controls resist ordinary copying and simultaneous use, but do not guarantee
protection against an administrator modifying the software or spoofing identifiers.
Session controls cannot establish who is physically using a device or prevent
people from deliberately sharing an unlocked browser or copied session credentials.
Each operator must keep their account and device access private.

## Operator access

The initial allowance is **20 registered / 5 active operators**, including **2
registered / 1 active local profiles** without Google. The publisher can configure
these limits per site. One stable identity has one central registration and one active browser session.
Tabs in the same browser share that session. Another browser must wait for sign-out
or expiry. Hiding or renaming a local profile does not free a registration; only
the publisher can suspend, revoke or restore central registrations.
The activation window shows the assigned limits. The manager displays working and
registered operators automatically; site details show all four counts and the
last online verification. Publisher changes arrive through the existing renewal.

Verified KM3NeT Google accounts require site approval. Other Google accounts cannot
sign in to inspections, but remain an option for separate Drive connections.
Local profiles require both site and publisher approval. Local identities are
site-declared, not Google-verified. Approval follows stable identity rather than
a display name. Signing in does not give an operator distributor privileges.

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

The installer and portable archive include installation and workflow guides, licence notices,
verification records and checksums. Consult those records for the checks performed
on the supplied executable. Physical cameras, hotspot adapters, real Google/Drive
accounts, desktop appearance and sustained load still require checks at each site.
Use **Menu → View activity** and `./VInspect --check-runtime` for diagnostics.

Application source, site records, credentials, private signing keys and the private
administration service are excluded from this public release repository.
