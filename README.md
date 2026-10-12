# VInspect releases

**VInspect 1.0.0** is the first official Linux release for visual inspection of
KM3NeT DOMs, detection units, production batches and electronic components.

Developed by **Emiliano Librizzi** · **INFN Naples** · **Capacity Laboratory** · **KM3NeT**.

## Download and install

Download [**VInspect-Setup**](https://github.com/emilianolibrizzi/vinspect-releases/releases/latest/download/VInspect-Setup)
and its [SHA-256 checksum](https://github.com/emilianolibrizzi/vinspect-releases/releases/latest/download/VInspect-Setup.sha256).
This **single executable** contains the application, bundled Python, guides,
licence and third-party notices. Open it, choose your language and installation
folder (default **~/VInspect**), then **Install → Continue setup**. The guided
installer includes progress and an optional Applications-menu shortcut.

Linux may require **Properties → Permissions → Allow executing file as program**
first. From a terminal in the download folder, use `chmod +x VInspect-Setup`, then
`./VInspect-Setup`. Do not use `sudo`. Setup needs no archive extraction, Python
installation or administrator privileges. It verifies the included files. For an
existing installation, close VInspect, select its folder and choose **Update
VInspect**: activation, settings and inspection files are kept. Do not delete the
old folder or create another site to update. A new installation gets fresh storage.
Moving a site to another computer remains a separate authorised transfer. Setup
removes its private temporary files when it closes.

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

After reviewing and accepting the licence, **Site activation** opens before the
server manager. Choose **Continue in browser**, sign in with your verified KM3NeT
Google account on the official page and select your site from the author's
directory. Return to the client and wait for the author's approval. The client
then verifies its signed licence and connects its managed update controls.

Only the author creates directory entries; renaming a site does not create another
licence or reset limits. One entry authorises one server, with separately approved
operator browsers. If your site is missing, contact
[Emiliano Librizzi](mailto:emiliano.librizzi@gmail.com). A private one-use activation
code supplied by the author remains a manual alternative. Google sign-in for the
request does not configure Google operator access or Drive on the local server.

A code normally expires after **24 hours** and activates one server computer.
Start a normal server transfer on the currently authorised computer. After
confirmation, its inspection service stops and its central authorisation is
suspended. Use its private, one-use transfer code and a verified KM3NeT Google
account on the new computer. Guided transfers are preauthorised by default and
complete automatically after the service verifies the handoff and new binding.
The author can disable this option per site, requiring manual review instead.
The site keeps its licence and operator limits. Cancelling the request does not reactivate the old server;
contact the author if the transfer must be reversed.

If the old computer is broken, submit a separate recovery request from the new
computer and contact the author. This request clearly lacks the old server's
approval and does not suspend or replace the existing installation. The author
must independently verify the request and explicitly approve recovery. Any
outstanding authorisation can require up to 60 minutes of waiting before the
replacement starts, preventing overlapping use.

Restore inspection projects from their backups separately; activation does not
copy files. Old activation files must not overwrite the new setup.

**Resume activation** recovers an interrupted exchange using the saved claim.
Cancelling setup closes the application without starting the server. After valid
activation, the manager can open offline for status and recovery; missing or
invalid activation returns to setup. The non-secret **Support reference** under
**Help** identifies the installation for assistance; it is not an
activation code. Existing files remain accessible through the file manager.
The inspection server requires a signed machine-bound licence and a
fresh online authorisation at every start. Multiple operator browsers may connect
to that server according to its local access policy.

Authorisation is renewed **every fifteen minutes** and lasts at most **60 minutes**. Brief
Internet interruptions are tolerated until expiry; then new protected work pauses
until verification succeeds. Existing files and recoverable browser drafts remain
intact. A replacement computer requires a verified transfer under the publisher’s
site policy, even if the complete archive was copied. Older offline-only grants require online activation.
Public availability does not grant unrestricted use or activate a site.

When all operators have been inactive for 30 minutes, the running server enters
standby and pauses periodic cloud authorisation checks. Open tabs and automatic
page polling do not count as human activity. Active uploads and saves keep the
server awake. Returning to work requires a fresh online authorisation; inspection
files and browser drafts remain intact. This idle threshold is separate from the
60-minute maximum validity of an authorisation during an Internet interruption.

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

**Menu → Site connection** shows the authorisation connection. If recovery is needed, **Site details** opens the authorised activation workflow directly. After activation, the client synchronises and checks for updates automatically. New sites inherit the publisher’s release policy; explicit site holds remain under publisher control. The distributed client cannot import another connection or disconnect this required service.
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
The activation window shows the assigned limits. Compact site, licence and
operator indicators summarise the manager's status; details show all four counts
and the last online verification. The display refreshes automatically, while
centrally verified counts and publisher changes arrive through background checks.
Historical or unavailable information is labelled accordingly, not shown as a
guaranteed live result.

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

The guided installer can update an existing installation while preserving its
activation and archive. A private registration also recognises the same computer
and Linux user when the program folder changes. If the original archive is
missing, activation recovery is separate from restoring inspection data. Online
server authorisation and approved transfers remain mandatory.
