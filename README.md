Demos Ra
========

I build plain-text data tools for AI agents and the people who work with
them. Every one rests on Multi-Sheet Tab-Separated Values (MTSV), a file
format specified in an IETF Internet-Draft: TSV with one more dimension,
where a tab separates fields, a line break separates records, and a form
feed separates sheets. A whole Excel (XLSX) workbook becomes one text file
that any AI agent, editor or script can read. Its media type,
text/prs.mtsv, is registered with IANA.

Why It Is Useful
----------------

AI agents read text. Excel workbooks, databases and agent memory are
usually binary or locked inside one tool, so an agent cannot see them whole.
MTSV keeps every sheet in plain text, so people, AI agents and ordinary
tools all read and change the same file.

Repositories
------------

* [mtsv-spec](https://github.com/demos-ra/mtsv-spec): the MTSV specification, an IETF Internet-Draft
  * [mtsv](https://github.com/demos-ra/mtsv): Python library and command that convert Excel, ODS, CSV, JSON, SQLite, Parquet and Arrow to and from MTSV
    * [mtsv-office](https://github.com/demos-ra/mtsv-office): open and save spreadsheets as MTSV in office apps: LibreOffice Calc now, Excel next
    * [text-spreadsheet](https://github.com/demos-ra/text-spreadsheet): MCP (Model Context Protocol) server that lets AI agents read Excel, CSV and other spreadsheets as text
    * [living-memory](https://github.com/demos-ra/living-memory): agent memory for any AI agent, as plain tables; Claude Code first
  * [living-architecture](https://github.com/demos-ra/living-architecture): code generation from small MTSV grids, for Next.js, TypeScript, React, Prisma, CSS and JSON
  * [void-os](https://github.com/demos-ra/void-os): the personal operating system for AI agents: memory, tools and hooks in one relational data bank of plain text

Linux Kernel
------------

* [457dc9fefe9a ("netlink: specs: Add a spec for nexthops in rtnetlink")](https://git.kernel.org/netdev/net-next/c/457dc9fefe9a): a YNL spec for nexthop objects and nexthop buckets in rtnetlink, applied to net-next by Jakub Kicinski in October 2026; [the patch on the netdev mailing list](https://lore.kernel.org/20261019-rt-nexthop-spec-v1-1-9c586edf86ab@gmail.com)

OpenClaw
--------

* [openclaw/openclaw@c00352f](https://github.com/openclaw/openclaw/commit/c00352f56c4982d2adf9f641d6abbadf3fa12daf): keeps the AppImage's bundled libraries out of the host programs the Linux companion starts, so an SSH ProxyCommand that loads the system OpenSSL no longer aborts; co-authored with Peter Steinberger, who merged it into main in October 2026; [the pull request on GitHub](https://github.com/openclaw/openclaw/pull/183661)

Get Started
-----------

* [Convert Excel and other files to MTSV](https://github.com/demos-ra/mtsv): `pipx install mtsv`
* [Let AI agents read Excel through an MCP server](https://github.com/demos-ra/text-spreadsheet): `pipx install text-spreadsheet`
* [Run the operating system for AI agents](https://github.com/demos-ra/void-os): `pipx install void-os` or `npm install --global void-os`

Get Help
--------

* Issues: the issue tracker of each repository
* Maintainer: Demos Ra
