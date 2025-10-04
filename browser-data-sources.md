---
title: Browser Data Sources
nav_order: 4
parent: Reference
---

## <center>Game Browser Data Sources</center>

The Game Browser gets its data from several sources, and it's not apparent which field comes from where.

The following fields are read directly from the Games:

- Filename (w/o extension)  
- CIC Chip  
- Country  
- CRC1  
- CRC2  
- Internal Name  
- Manufacturer  
- Game size

The following fields are read from `MiB64.rds`:

- Game Name  
- Status  
- Notes (Core)  
- Notes (Plugins)

The following fields are read from `MiB64.rdi` (if available):

- Developer  
- ForceFeedback  
- Game Information (URL Link)  
- Game Language  
- Genre  
- Players  
- Release Date

The following fields are read from `MiB64.rdn` (if available):

- Notes (User)

Any data not available will simply appear blank.

---

<!-- Footer Navigation Block -->

<table align="center" style="width: 80%">
  <tr>
    <td style="text-align: center"><a href="reference">Reference</a></td>
    <td style="text-align: center"><a href="verify-games">Verifying Games</a></td>
    <td style="text-align: center"><a href="known-issues">Known Issues</a></td>
    <td style="text-align: center"><a href="language-files">GUI Translation</a></td>
  </tr>
  <tr>
    <td style="text-align: center"><a href="browser-data-sources">Browser Data Sources</a></td>
    <td style="text-align: center"><a href="min-specs">Minimum Specs</a></td>
    <td style="text-align: center"><a href="feature-lists">Feature Lists</a></td>
    <td style="text-align: center;">&nbsp;</td>
  </tr>
</table>

<p style="text-align:center"><a href="#">Return to the top</a></p>

<!-- ClauseEcho: Browser Data Sources Protocol Activated -->
